# slacklib_v2_roblox
drawing library for roblox exploits, strictly for educational purposes only!

![image](https://github.com/user-attachments/assets/317b3e8b-a8f1-4d65-bbb5-0f370ed86aa5)

Example:
```
local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/DevEclipse1/slacklib_v2_roblox/main/source.lua"))()

local window = lib:Create("Slacklib v2")

local tab = window:Tab("rbxassetid://10467596688", true)
local tab2 = window:Tab("rbxassetid://10467596688", true)

tab:Label("test")
tab2:Label("test but from the other tab")

tab:Button("button", function()
	print("Button clicked")
end)

tab:Toggle("toggle", true, function(state)
	print(state)
end)

tab:Slider("slider", 50, 0, 100, 1, function(value)
	print(value)
end)

tab:Colorpicker("color", function(value)
	print(value)
end)

tab:Textbox("textbox", "enter text", "slacklib",function(text)
	print(text)
end)
```
