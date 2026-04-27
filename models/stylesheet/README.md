# stylesheet
* Roblox Studio version: 0.718.0.7181104

Contains a `StyleSheet` with two `StyleRule` children that exercise `PropertiesSerialize` and `PropertyTransitionsSerialize`.

- First StyleRule (selector: `Frame`):
  - `PropertiesSerialize`: Attributes with `Size = UDim2(1, 0, 0.5, 0)`
  - `PropertyTransitionsSerialize`: Attributes with `Size = TweenInfo(0.2, Exponential, Out)`, prefixed with `02 00` discriminant.
- Second StyleRule (selector: `:hover`):
  - `PropertiesSerialize`: Attributes with `Size = UDim2(1, 0, 0.85, 0)`
  - `PropertyTransitionsSerialize`: Empty attributes, prefixed with `02 00` discriminant.
