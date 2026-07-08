---
title: KeyCode
type: enum
---

# `Enum.KeyCode`

Byte keycodes that represent the key or button involved in user input.

The `KeyCode` enum contains a list of byte keycodes that represent the key or
button involved in user input. This enum also includes buttons and axes
present on gamepads, and 96 `World[]` values for non-standard buttons.

Note that keyboard values refer to the physical position of buttons on a
standard QWERTY keyboard. Provided the user's system is configured correctly,
the location of keys (such as
<kbd>W</kbd><kbd>A</kbd><kbd>S</kbd><kbd>D</kbd>) will remain the same on
other keyboard types such as Dvorak keyboards where it would map to
<kbd>,</kbd><kbd>A</kbd><kbd>O</kbd><kbd>E</kbd>.

See also `Class.InputObject`, used for keyboard and gamepad input.

The `Enum.KeyCode` enum has 277 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.KeyCode.Unknown` | 0 | Blank value that represents no key being pressed. |
| `Enum.KeyCode.Backspace` | 8 | The `Backspace` key. |
| `Enum.KeyCode.Tab` | 9 | The `Tab` key. |
| `Enum.KeyCode.Clear` | 12 | Only present on certain keyboards. |
| `Enum.KeyCode.Return` | 13 | Frequently known as **Enter**. |
| `Enum.KeyCode.Pause` | 19 | Only present on certain keyboards. |
| `Enum.KeyCode.Escape` | 27 | The `Escape` key. |
| `Enum.KeyCode.Space` | 32 | The `Space` key. |
| `Enum.KeyCode.QuotedDouble` | 34 | The `"` key. |
| `Enum.KeyCode.Hash` | 35 | The `#` key. |
| `Enum.KeyCode.Dollar` | 36 | The `$` key. |
| `Enum.KeyCode.Percent` | 37 | The `%` key. |
| `Enum.KeyCode.Ampersand` | 38 | The `&` key. |
| `Enum.KeyCode.Quote` | 39 | The `'` key. |
| `Enum.KeyCode.LeftParenthesis` | 40 | The `(` key. |
| `Enum.KeyCode.RightParenthesis` | 41 | The `)` key. |
| `Enum.KeyCode.Asterisk` | 42 | The `*` key. |
| `Enum.KeyCode.Plus` | 43 | The `+` key. |
| `Enum.KeyCode.Comma` | 44 | The `,` key. |
| `Enum.KeyCode.Minus` | 45 | The `-` key. |
| `Enum.KeyCode.Period` | 46 | The `.` key. |
| `Enum.KeyCode.Slash` | 47 | The `/` key. |
| `Enum.KeyCode.Zero` | 48 | The `0` key. |
| `Enum.KeyCode.One` | 49 | The `1` key. |
| `Enum.KeyCode.Two` | 50 | The `2` key. |
| `Enum.KeyCode.Three` | 51 | The `3` key. |
| `Enum.KeyCode.Four` | 52 | The `4` key. |
| `Enum.KeyCode.Five` | 53 | The `5` key. |
| `Enum.KeyCode.Six` | 54 | The `6` key. |
| `Enum.KeyCode.Seven` | 55 | The `7` key. |
| `Enum.KeyCode.Eight` | 56 | The `8` key. |
| `Enum.KeyCode.Nine` | 57 | The `9` key. |
| `Enum.KeyCode.Colon` | 58 | The `:` key. |
| `Enum.KeyCode.Semicolon` | 59 | The `;` key. |
| `Enum.KeyCode.LessThan` | 60 | The `<` key. |
| `Enum.KeyCode.Equals` | 61 | The `=` key. |
| `Enum.KeyCode.GreaterThan` | 62 | The `>` key. |
| `Enum.KeyCode.Question` | 63 | The `?` key. |
| `Enum.KeyCode.At` | 64 | The `@` key. |
| `Enum.KeyCode.LeftBracket` | 91 | The `[` key. |
| `Enum.KeyCode.BackSlash` | 92 | The `\` key. |
| `Enum.KeyCode.RightBracket` | 93 | The `]` key. |
| `Enum.KeyCode.Caret` | 94 | The `^` key. |
| `Enum.KeyCode.Underscore` | 95 | The `_` key. |
| `Enum.KeyCode.Backquote` | 96 | The `` ` `` key. |
| `Enum.KeyCode.A` | 97 | The `A` key. |
| `Enum.KeyCode.B` | 98 | The `B` key. |
| `Enum.KeyCode.C` | 99 | The `C` key. |
| `Enum.KeyCode.D` | 100 | The `D` key. |
| `Enum.KeyCode.E` | 101 | The `E` key. |
| `Enum.KeyCode.F` | 102 | The `F` key. |
| `Enum.KeyCode.G` | 103 | The `G` key. |
| `Enum.KeyCode.H` | 104 | The `H` key. |
| `Enum.KeyCode.I` | 105 | The `I` key. |
| `Enum.KeyCode.J` | 106 | The `J` key. |
| `Enum.KeyCode.K` | 107 | The `K` key. |
| `Enum.KeyCode.L` | 108 | The `L` key. |
| `Enum.KeyCode.M` | 109 | The `M` key. |
| `Enum.KeyCode.N` | 110 | The `N` key. |
| `Enum.KeyCode.O` | 111 | The `O` key. |
| `Enum.KeyCode.P` | 112 | The `P` key. |
| `Enum.KeyCode.Q` | 113 | The `Q` key. |
| `Enum.KeyCode.R` | 114 | The `R` key. |
| `Enum.KeyCode.S` | 115 | The `S` key. |
| `Enum.KeyCode.T` | 116 | The `T` key. |
| `Enum.KeyCode.U` | 117 | The `U` key. |
| `Enum.KeyCode.V` | 118 | The `V` key. |
| `Enum.KeyCode.W` | 119 | The `W` key. |
| `Enum.KeyCode.X` | 120 | The `X` key. |
| `Enum.KeyCode.Y` | 121 | The `Y` key. |
| `Enum.KeyCode.Z` | 122 | The `Z` key. |
| `Enum.KeyCode.LeftCurly` | 123 | The `{` key. |
| `Enum.KeyCode.Pipe` | 124 | The `/` key. |
| `Enum.KeyCode.RightCurly` | 125 | The `}` key. |
| `Enum.KeyCode.Tilde` | 126 | The `~` key. |
| `Enum.KeyCode.Delete` | 127 | The `Del` key. |
| `Enum.KeyCode.World0` | 160 |  |
| `Enum.KeyCode.World1` | 161 |  |
| `Enum.KeyCode.World2` | 162 |  |
| `Enum.KeyCode.World3` | 163 |  |
| `Enum.KeyCode.World4` | 164 |  |
| `Enum.KeyCode.World5` | 165 |  |
| `Enum.KeyCode.World6` | 166 |  |
| `Enum.KeyCode.World7` | 167 |  |
| `Enum.KeyCode.World8` | 168 |  |
| `Enum.KeyCode.World9` | 169 |  |
| `Enum.KeyCode.World10` | 170 |  |
| `Enum.KeyCode.World11` | 171 |  |
| `Enum.KeyCode.World12` | 172 |  |
| `Enum.KeyCode.World13` | 173 |  |
| `Enum.KeyCode.World14` | 174 |  |
| `Enum.KeyCode.World15` | 175 |  |
| `Enum.KeyCode.World16` | 176 |  |
| `Enum.KeyCode.World17` | 177 |  |
| `Enum.KeyCode.World18` | 178 |  |
| `Enum.KeyCode.World19` | 179 |  |
| `Enum.KeyCode.World20` | 180 |  |
| `Enum.KeyCode.World21` | 181 |  |
| `Enum.KeyCode.World22` | 182 |  |
| `Enum.KeyCode.World23` | 183 |  |
| `Enum.KeyCode.World24` | 184 |  |
| `Enum.KeyCode.World25` | 185 |  |
| `Enum.KeyCode.World26` | 186 |  |
| `Enum.KeyCode.World27` | 187 |  |
| `Enum.KeyCode.World28` | 188 |  |
| `Enum.KeyCode.World29` | 189 |  |
| `Enum.KeyCode.World30` | 190 |  |
| `Enum.KeyCode.World31` | 191 |  |
| `Enum.KeyCode.World32` | 192 |  |
| `Enum.KeyCode.World33` | 193 |  |
| `Enum.KeyCode.World34` | 194 |  |
| `Enum.KeyCode.World35` | 195 |  |
| `Enum.KeyCode.World36` | 196 |  |
| `Enum.KeyCode.World37` | 197 |  |
| `Enum.KeyCode.World38` | 198 |  |
| `Enum.KeyCode.World39` | 199 |  |
| `Enum.KeyCode.World40` | 200 |  |
| `Enum.KeyCode.World41` | 201 |  |
| `Enum.KeyCode.World42` | 202 |  |
| `Enum.KeyCode.World43` | 203 |  |
| `Enum.KeyCode.World44` | 204 |  |
| `Enum.KeyCode.World45` | 205 |  |
| `Enum.KeyCode.World46` | 206 |  |
| `Enum.KeyCode.World47` | 207 |  |
| `Enum.KeyCode.World48` | 208 |  |
| `Enum.KeyCode.World49` | 209 |  |
| `Enum.KeyCode.World50` | 210 |  |
| `Enum.KeyCode.World51` | 211 |  |
| `Enum.KeyCode.World52` | 212 |  |
| `Enum.KeyCode.World53` | 213 |  |
| `Enum.KeyCode.World54` | 214 |  |
| `Enum.KeyCode.World55` | 215 |  |
| `Enum.KeyCode.World56` | 216 |  |
| `Enum.KeyCode.World57` | 217 |  |
| `Enum.KeyCode.World58` | 218 |  |
| `Enum.KeyCode.World59` | 219 |  |
| `Enum.KeyCode.World60` | 220 |  |
| `Enum.KeyCode.World61` | 221 |  |
| `Enum.KeyCode.World62` | 222 |  |
| `Enum.KeyCode.World63` | 223 |  |
| `Enum.KeyCode.World64` | 224 |  |
| `Enum.KeyCode.World65` | 225 |  |
| `Enum.KeyCode.World66` | 226 |  |
| `Enum.KeyCode.World67` | 227 |  |
| `Enum.KeyCode.World68` | 228 |  |
| `Enum.KeyCode.World69` | 229 |  |
| `Enum.KeyCode.World70` | 230 |  |
| `Enum.KeyCode.World71` | 231 |  |
| `Enum.KeyCode.World72` | 232 |  |
| `Enum.KeyCode.World73` | 233 |  |
| `Enum.KeyCode.World74` | 234 |  |
| `Enum.KeyCode.World75` | 235 |  |
| `Enum.KeyCode.World76` | 236 |  |
| `Enum.KeyCode.World77` | 237 |  |
| `Enum.KeyCode.World78` | 238 |  |
| `Enum.KeyCode.World79` | 239 |  |
| `Enum.KeyCode.World80` | 240 |  |
| `Enum.KeyCode.World81` | 241 |  |
| `Enum.KeyCode.World82` | 242 |  |
| `Enum.KeyCode.World83` | 243 |  |
| `Enum.KeyCode.World84` | 244 |  |
| `Enum.KeyCode.World85` | 245 |  |
| `Enum.KeyCode.World86` | 246 |  |
| `Enum.KeyCode.World87` | 247 |  |
| `Enum.KeyCode.World88` | 248 |  |
| `Enum.KeyCode.World89` | 249 |  |
| `Enum.KeyCode.World90` | 250 |  |
| `Enum.KeyCode.World91` | 251 |  |
| `Enum.KeyCode.World92` | 252 |  |
| `Enum.KeyCode.World93` | 253 |  |
| `Enum.KeyCode.World94` | 254 |  |
| `Enum.KeyCode.World95` | 255 |  |
| `Enum.KeyCode.KeypadZero` | 256 | The `0` key on the keypad cluster. |
| `Enum.KeyCode.KeypadOne` | 257 | The `1` key on the keypad cluster. |
| `Enum.KeyCode.KeypadTwo` | 258 | The `2` key on the keypad cluster. |
| `Enum.KeyCode.KeypadThree` | 259 | The `3` key on the keypad cluster. |
| `Enum.KeyCode.KeypadFour` | 260 | The `4` key on the keypad cluster. |
| `Enum.KeyCode.KeypadFive` | 261 | The `5` key on the keypad cluster. |
| `Enum.KeyCode.KeypadSix` | 262 | The `6` key on the keypad cluster. |
| `Enum.KeyCode.KeypadSeven` | 263 | The `7` key on the keypad cluster. |
| `Enum.KeyCode.KeypadEight` | 264 | The `8` key on the keypad cluster. |
| `Enum.KeyCode.KeypadNine` | 265 | The `9` key on the keypad cluster. |
| `Enum.KeyCode.KeypadPeriod` | 266 | The `.` key on the keypad cluster. |
| `Enum.KeyCode.KeypadDivide` | 267 | The `/` key on the keypad cluster. |
| `Enum.KeyCode.KeypadMultiply` | 268 | The `*` key on the keypad cluster. |
| `Enum.KeyCode.KeypadMinus` | 269 | The `-` key on the keypad cluster. |
| `Enum.KeyCode.KeypadPlus` | 270 | The `+` key on the keypad cluster. |
| `Enum.KeyCode.KeypadEnter` | 271 | The `Enter` key on the keypad cluster. |
| `Enum.KeyCode.KeypadEquals` | 272 | The `=` key on the keypad cluster. |
| `Enum.KeyCode.Up` | 273 | The `↑` arrow key. |
| `Enum.KeyCode.Down` | 274 | The `↓` arrow key. |
| `Enum.KeyCode.Right` | 275 | The `→` arrow key. |
| `Enum.KeyCode.Left` | 276 | The `←` arrow key. |
| `Enum.KeyCode.Insert` | 277 | The `Insert` key. |
| `Enum.KeyCode.Home` | 278 | The `Home` key. |
| `Enum.KeyCode.End` | 279 | The `End` key. |
| `Enum.KeyCode.PageUp` | 280 | The `PgUp` key. |
| `Enum.KeyCode.PageDown` | 281 | The `PgDown` key. |
| `Enum.KeyCode.F1` | 282 | The `F1` key. |
| `Enum.KeyCode.F2` | 283 | The `F2` key. |
| `Enum.KeyCode.F3` | 284 | The `F3` key. |
| `Enum.KeyCode.F4` | 285 | The `F4` key. |
| `Enum.KeyCode.F5` | 286 | The `F5` key. |
| `Enum.KeyCode.F6` | 287 | The `F6` key. |
| `Enum.KeyCode.F7` | 288 | The `F7` key. |
| `Enum.KeyCode.F8` | 289 | The `F8` key. |
| `Enum.KeyCode.F9` | 290 | The `F9` key. |
| `Enum.KeyCode.F10` | 291 | The `F10` key. |
| `Enum.KeyCode.F11` | 292 | The `F11` key. |
| `Enum.KeyCode.F12` | 293 | The `F12` key. |
| `Enum.KeyCode.F13` | 294 | The `F13` key. Only present on certain keyboards. |
| `Enum.KeyCode.F14` | 295 | The `F14` key. Only present on certain keyboards. |
| `Enum.KeyCode.F15` | 296 | The `F15` key. Only present on certain keyboards. |
| `Enum.KeyCode.NumLock` | 300 | The `Num Lock` key on the keypad cluster. |
| `Enum.KeyCode.CapsLock` | 301 | The `Caps Lock` key. |
| `Enum.KeyCode.ScrollLock` | 302 | The `Scr Lock` key. |
| `Enum.KeyCode.RightShift` | 303 | The right side `Shift` key. |
| `Enum.KeyCode.LeftShift` | 304 | The left side `Shift` key. |
| `Enum.KeyCode.RightControl` | 305 | The right side `Ctrl` key. |
| `Enum.KeyCode.LeftControl` | 306 | The left side `Ctrl` key. |
| `Enum.KeyCode.RightAlt` | 307 | The right side `Alt` key. |
| `Enum.KeyCode.LeftAlt` | 308 | The left side `Alt` key. |
| `Enum.KeyCode.RightMeta` | 309 | The right side `Meta` key. |
| `Enum.KeyCode.LeftMeta` | 310 | The left side `Meta` key. |
| `Enum.KeyCode.LeftSuper` | 311 | The left side `Super` key. Better known as the Windows key or <kbd>Cmd</kbd> key. |
| `Enum.KeyCode.RightSuper` | 312 | The right side `Super` key. Better known as the Windows key or <kbd>Cmd</kbd> key. |
| `Enum.KeyCode.Mode` | 313 | Only present on certain keyboards. |
| `Enum.KeyCode.Compose` | 314 | Only present on certain keyboards. |
| `Enum.KeyCode.Help` | 315 | Only present on certain keyboards. |
| `Enum.KeyCode.Print` | 316 | Only present on certain keyboards. |
| `Enum.KeyCode.SysReq` | 317 | Only present on certain keyboards. |
| `Enum.KeyCode.Break` | 318 | Only present on certain keyboards. |
| `Enum.KeyCode.Menu` | 319 | The `Menu` key. |
| `Enum.KeyCode.Power` | 320 | Only present on certain keyboards. |
| `Enum.KeyCode.Euro` | 321 | The `€` key. Only present on certain keyboards. |
| `Enum.KeyCode.Undo` | 322 | Only present on certain keyboards. |
| `Enum.KeyCode.ButtonX` | 1000 | Gamepad `X` button. |
| `Enum.KeyCode.ButtonY` | 1001 | Gamepad `Y` button. |
| `Enum.KeyCode.ButtonA` | 1002 | Gamepad `A` button. |
| `Enum.KeyCode.ButtonB` | 1003 | Gamepad `B` button. |
| `Enum.KeyCode.ButtonR1` | 1004 | Gamepad `R1` button. |
| `Enum.KeyCode.ButtonL1` | 1005 | Gamepad `L1` button. |
| `Enum.KeyCode.ButtonR2` | 1006 | Gamepad `R2` button. |
| `Enum.KeyCode.ButtonL2` | 1007 | Gamepad `L2` button. |
| `Enum.KeyCode.ButtonR3` | 1008 | Gamepad `R3` button. |
| `Enum.KeyCode.ButtonL3` | 1009 | Gamepad `L3` button. |
| `Enum.KeyCode.ButtonStart` | 1010 | Gamepad `Start` button. |
| `Enum.KeyCode.ButtonSelect` | 1011 | Gamepad `Select` button. |
| `Enum.KeyCode.DPadLeft` | 1012 | Left arrow on a gamepad D-pad. |
| `Enum.KeyCode.DPadRight` | 1013 | Right arrow on a gamepad D-pad. |
| `Enum.KeyCode.DPadUp` | 1014 | Up arrow on a gamepad D-pad. |
| `Enum.KeyCode.DPadDown` | 1015 | Down arrow on a gamepad D-pad. |
| `Enum.KeyCode.Thumbstick1` | 1016 | Gamepad primary thumbstick. |
| `Enum.KeyCode.Thumbstick2` | 1017 | Gamepad secondary thumbstick. |
| `Enum.KeyCode.Thumbstick1Up` | 1018 | Up vector on the gamepad primary thumbstick. Primarily used in the [Input Action System](../../../in |
| `Enum.KeyCode.Thumbstick1Down` | 1019 | Down vector on the gamepad primary thumbstick. Primarily used in the [Input Action System](../../../ |
| `Enum.KeyCode.Thumbstick1Left` | 1020 | Left vector on the gamepad primary thumbstick. Primarily used in the [Input Action System](../../../ |
| `Enum.KeyCode.Thumbstick1Right` | 1021 | Right vector on the gamepad primary thumbstick. Primarily used in the [Input Action System](../../.. |
| `Enum.KeyCode.Thumbstick2Up` | 1022 | Up vector on the gamepad secondary thumbstick. Primarily used in the [Input Action System](../../../ |
| `Enum.KeyCode.Thumbstick2Down` | 1023 | Down vector on the gamepad secondary thumbstick. Primarily used in the [Input Action System](../../. |
| `Enum.KeyCode.Thumbstick2Left` | 1024 | Left vector on the gamepad secondary thumbstick. Primarily used in the [Input Action System](../../. |
| `Enum.KeyCode.Thumbstick2Right` | 1025 | Right vector on the gamepad secondary thumbstick. Primarily used in the [Input Action System](../../ |
| `Enum.KeyCode.MouseLeftButton` | 1026 | The left mouse button, also commonly referred to as "button 1" on a generic mouse. Primarily used in |
| `Enum.KeyCode.MouseRightButton` | 1027 | The right mouse button, also commonly referred to as "button 2" on a generic mouse. Primarily used i |
| `Enum.KeyCode.MouseMiddleButton` | 1028 | The middle mouse button, also commonly referred to as "button 3" on a generic mouse. Primarily used  |
| `Enum.KeyCode.MouseBackButton` | 1029 |  |
| `Enum.KeyCode.MouseNoButton` | 1030 |  |
| `Enum.KeyCode.MouseX` | 1031 |  |
| `Enum.KeyCode.MouseY` | 1032 |  |
| `Enum.KeyCode.MousePosition` | 1033 | The position of a mouse in the viewport. Primarily used in the [Input Action System](../../../input/ |
| `Enum.KeyCode.TouchPosition` | 1034 | The position of a touch in the viewport. Primarily used in the [Input Action System](../../../input/ |
| `Enum.KeyCode.MouseWheel` | 1035 | The scroll delta (change) of a mouse wheel. Primarily used in the [Input Action System](../../../inp |
| `Enum.KeyCode.TrackpadPan` | 1040 | The pan delta (change) from a trackpad two-finger pan gesture. Primarily used in the [Input Action S |
| `Enum.KeyCode.TrackpadPinch` | 1045 | The scale delta (change) from a trackpad two-finger pinch gesture. Primarily used in the [Input Acti |
| `Enum.KeyCode.MouseDelta` | 1048 | The movement delta (change) of the mouse cursor. Primarily used in the [Input Action System](../../. |
| `Enum.KeyCode.TouchDelta` | 1049 | The movement delta (change) of a touch input. Primarily used in the [Input Action System](../../../i |
| `Enum.KeyCode.TouchPinch` | 1050 | The scale delta (change) of a two-finger touch pinch gesture. Primarily used in the [Input Action Sy |
