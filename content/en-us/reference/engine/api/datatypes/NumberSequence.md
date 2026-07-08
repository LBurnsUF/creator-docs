---
title: NumberSequence
type: datatype
---

# `Datatype.NumberSequence`

A series of floats across a period of time.

## Description

The `Datatype.NumberSequence` data type represents a series of number values
from `0` to `1`. The number values are expressed using the
`Datatype.NumberSequenceKeypoint` type. This type is used in properties such
as `Class.ParticleEmitter.Size` and `Class.Beam.Transparency` to define a
numerical change over time.

#### Equality

Two `Datatype.NumberSequence` objects are equivalent only if the values of
their `Datatype.NumberSequenceKeypoint` are equivalent, even if both would
result in similar graphs.

#### Evaluation

The `Datatype.NumberSequence` type does not have a built-in method for getting
the value at a certain time/point because keypoints can have random envelopes.
However, assuming the envelope values of your keypoints are all `0`, you can
use the following function to evaluate at a specific time.

```lua
local function evalNumberSequence(sequence: NumberSequence, time: number)
    -- If time is 0 or 1, return the first or last value respectively
    if time == 0 then
        return sequence.Keypoints[1].Value
    elseif time == 1 then
        return sequence.Keypoints[#sequence.Keypoints].Value
    end

    -- Otherwise, step through each sequential pair of keypoints
    for i = 1, #sequence.Keypoints - 1 do
        local currKeypoint = sequence.Keypoints[i]
        local nextKeypoint = sequence.Keypoints[i + 1]
        if time >= currKeypoint.Time and time < nextKeypoint.Time then
            -- Calculate how far alpha lies between the points
            local alpha = (time - currKeypoint.Time) / (nextKeypoint.Time - currKeypoint.Time)
            -- Return the value between the points using alpha
            return currKeypoint.Value + (nextKeypoint.Value - currKeypoint.Value) * alpha
        end
    end
end

local numberSequence = NumberSequence.new{
    NumberSequenceKeypoint.new(0, 0),
    NumberSequenceKeypoint.new(0.5, 1),
    NumberSequenceKeypoint.new(1, 0),
}

print(evalNumberSequence(numberSequence, 0.65))  --> 0.7
```

## Constructors

### `NumberSequence.new`

Returns a `Datatype.NumberSequence` with the start and end values set to
the provided `n`.

  ```lua
  local numberSequence = NumberSequence.new(n)
  -- Equivalent to
  local numberSequence = NumberSequence.new{
      NumberSequenceKeypoint.new(0, n),
      NumberSequenceKeypoint.new(1, n)
  }
  ```

**Parameters:**

- `n`: `number`

### `NumberSequence.new`

Returns a `Datatype.NumberSequence` of two keypoints with `n0` as the start value
and `n1` as the end value.

  ```lua
  local numberSequence = NumberSequence.new(n0, n1)
  -- Equivalent to
  local numberSequence = NumberSequence.new{
      NumberSequenceKeypoint.new(0, n0),
      NumberSequenceKeypoint.new(1, n1)
  }
  ```

**Parameters:**

- `n0`: `number`
- `n1`: `number`

### `NumberSequence.new`

Returns a `Datatype.NumberSequence` from an array of
`Datatype.NumberSequenceKeypoint|NumberSequenceKeypoints`. The keypoints
must be provided in a non-descending time value order. At least two keypoints must
be provided, and they must have a time value of `0` (first) and `1`
(last).

  ```lua
  local numberSequence = NumberSequence.new{
      NumberSequenceKeypoint.new(0, 0),
      NumberSequenceKeypoint.new(0.5, 0.5, 0.25),
      NumberSequenceKeypoint.new(1, 1)
  }
  ```

**Parameters:**

- `Keypoints`: `Array`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `NumberSequence.Keypoints` | `Array` | An array of `Datatype.NumberSequenceKeypoint` values in ascending order. |

## API Usage (7 locations)

### Used as Property Type

- `Class.Beam.Transparency`
- `Class.ParticleEmitter.Size`
- `Class.ParticleEmitter.Squash`
- `Class.ParticleEmitter.Transparency`
- `Class.Trail.Transparency`
- `Class.Trail.WidthScale`
- `Class.UIGradient.Transparency`
