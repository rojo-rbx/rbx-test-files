* Roblox Studio version: 0.566.0.5660545

Contains a tree like the following:

* `ScreenGui` with `IgnoreGuiInset = true`
* `ScreenGui` with `IgnoreGuiInset = false`
  * `TextLabel` with `Font = Enum.Font.Code (10)`
  * `TextLabel` with `Font = Enum.Font.SourceSansBold (4)`
  * `TextLabel` with `Font = Enum.Font.SourceSansItalic (6)`

This is used to test that the `IgnoreGuiInset -> ScreenInsets` and `Font -> FontFace` migrations work properly.

On read, rbx_dom should transform this into:

* `ScreenGui` with `ScreenInsets = CoreUISafeInsets (2)`
* `ScreenGui` with `ScreenInsets = DeviceSafeInsets (1)`
  * `TextLabel` with `Font = { family: Inconsolata ("rbxasset://fonts/families/Inconsolata.json"), weight: Regular (400), style: Normal (0) }`
  * `TextLabel` with `Font = { family: Inconsolata ("rbxasset://fonts/families/SourceSansPro.json"), weight: Bold (700), style: Normal (0) }`
  * `TextLabel` with `Font = { family: Inconsolata ("rbxasset://fonts/families/SourceSansPro.json"), weight: Regular (400), style: Italic (1) }`