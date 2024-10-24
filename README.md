# Pepsi UI Library (not mine)

Pepsi UI Library for Roblox | With documentation (look below)


## Load the Library
```lua
local library = loadstring(game:HttpGet('https://raw.githubusercontent.com/Stratxgy/PepsiUI/refs/heads/main/pepsi.lua'))()
```

## Create a Window
```lua
local ExampleHub = Library:CreateWindow({
	Name = "Example Hub",
	Themeable = {
		Image = "nil. -- Add roblox image id or remove this",
		Info = "Info",
		Credit = false
	},
	Background = "",
	-- if you want to turn off background put it here
})
```

## Turn off Background Image
```lua
Theme = [[{"__Designer.Background.UseBackgroundImage":false}]]
```

## Create a new Tab
```lua
local GeneralTab = ExampleHub:CreateTab({
Name = "General"
})
```

> [!IMPORTANT]
> Where " Side = "Left " is, you can change this to right for it to be on the right side.

## Create a Section
```lua
local ExampleSection = GeneralTab:CreateSection({
Name = "This is an example"
Side = "Left"
Callback = function()
Print("Example Print")
})
```



## Create a Toggle
```lua
ExampleSection:AddToggle({
Name = "Example toggle",
Side = "Left"
Callback = function()
Print("Example Print")
})
```

## Create a Slider
```lua
ExampleSection:AddSlider({
Name = "Example",
Value = 0.15,
Precise = 2,
Min = 0,
Max = 1
Side = "Left"
Callback = function()
Print("Example Print")
})
```

## Create a Keybind
```lua
ExampleSection:AddKeybind({
Name = "Example Key",
Callback = print
Side = "Left"
Callback = function()
Print("Example Print")
})
```


