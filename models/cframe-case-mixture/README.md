# cframe-case-mixture
* Roblox Studio version: 0.452.2.413165

Contains two `CFrameValue` objects with two seperate values and their names set accordingly. The values are:
    - `0, 0, 0, 1, 0, 0, 0, 0, -1, 0, 1, 0`
    - `0.15625, -0.15625, 0.1, -0.1, 0, 0, 1337, -1337, inf, -inf, nan, nan`

In the binary format, the first of these values will have an orientation ID of `03` and the second will have an orienation ID of `00`.

This test file is really only useful for testing implementations of the binary format, but an xml file is included for completion.