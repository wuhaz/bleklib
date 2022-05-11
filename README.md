# BlekLib

BlekLib is a open sourced Roblox UI library inspired by Dark Hub

## Loadstring
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/bleklib/main/library.lua"))()
```

## Features:
- Buttons
- Sliders
- Textbox
- Toggles
- Labels

more coming soon

Created by 'j#6066
My server: https://discord.gg/mwfAyYZ57P

## Documentation

### Loadstring
```lua
local BlekLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/laderite/bleklib/main/library.lua"))()
```

### Create the GUI
```lua
local win = Library:Create({
    Name = "Blek Library",
    StartupSound = {
        Toggle = false,
        SoundID = "rbxassetid://6958727243",
        TimePosition = 1
    }
})
```

### Tabs
```lua
local maintab = win:Tab('Main')
local charactertab = win:Tab('Character')
local uitab = win:Tab('UI')
```

### Buttons
```lua
uitab:Button('Destroy GUI', function()
    win:Exit()
end)
```

### Toggles
```lua
maintab:Toggle('Aimbot', function(v)
    aimbot = v
end)
```

### Textboxes
```lua
maintab:Textbox('FOV', function(v)
    fov = v
end)
```

### Sliders
```lua
maintab:Slider('FOV', 30 -- default, 10 -- min, 300 -- max, function(a)
    print(a)
end)
```

### Labels
```lua
maintab:Label('This is a label')
```
