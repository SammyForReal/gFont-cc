# gFont-cc
gFont is a 'small' API that draws text on enabled graphicsMode in CC:Tweaked.

There is a default font with the API, that supports the chars from ``\000`` to ``\159``. Its 9x9px big.

### Example:
```lua
local gFont = require("gFont")
---------------------------------------
term.setGraphicsMode(1)
term.clear()

term.setTextColor(colors.purple)
gFont.write(0,0,"The default font! :)")

term.setTextColor(colors.lightGray)
gFont.write(0,9,("\131"):rep(20))
sleep(1)
```
![Alt Text](/default-font-example.png "Screenshot the font")

> 👉Note: The API only works if **CC** supports the graphics mode! The original mod or normal emulators dont have this feature normally!
