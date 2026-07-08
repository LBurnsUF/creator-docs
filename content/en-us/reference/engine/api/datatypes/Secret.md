---
title: Secret
type: datatype
---

# `Datatype.Secret`

Stores secret non-printable content.

## Description

The `Datatype.Secret` data type stores the secret content returned by
`Class.HttpService:GetSecret()`. It cannot be printed or logged, but can be
modified using built-in functions:

```lua
local HttpService = game:GetService("HttpService")

local mySiteApiKey = HttpService:GetSecret("my_site")
local url = "https://apis.mysite.com?apiKey="
local urlWithKey = mySiteApiKey:AddPrefix(url)
local params = "&request=join&user=myname"
local resultingUrl = urlWithKey:AddSuffix(params)
```

## Methods

### `Secret:AddPrefix`

Returns a secret formed by concatenating the supplied string to the secret
content, for example prepending `"Bearer"` to the API key.

```lua
local HttpService = game:GetService("HttpService")

local secret = HttpService:GetSecret("yelp")
local authHeader = secret:AddPrefix("Bearer ")
```

**Parameters:**

- `prefix`: `string`

### `Secret:AddSuffix`

Returns a secret formed by concatenating the original secret and the
supplied string parameter. Useful when creating a URL containing a key and
query parameters.

```lua
local HttpService = game:GetService("HttpService")

local googleMapsApiKey = HttpService:GetSecret("google_map")

local baseUrl = "https://maps.googleapis.com/maps/api/distancematrix/json?key="
local queryParams = "&destinations=" .. destination .. "&origins=" .. origin .. "&departure_time=now&units=imperial"
local authedUrl = googleMapsApiKey:AddPrefix(baseUrl)
local queryUrl = authedUrl:AddSuffix(queryParams)
```

**Parameters:**

- `suffix`: `string`

## API Usage (2 locations)

### Used as Return Type

- `Class.HttpService:GetSecret`
- `Class.HttpService:RequestAccessTokenScopesAsync`
