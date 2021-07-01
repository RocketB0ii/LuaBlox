# How to make Plugins

Making plugins are simple.
let's test first

## Test
Add a new Script and write:
```lua
print("Plugin is active.")
```

Look in your output, and it should prints (If not, create an issue):
```lua
Plugin is active.
```

## Create a button
Now that it works, let's make a toolbox and a button, also this is simple as well...
We'll need a toolbox just to create a button

(plugin:CreateToolbox(ToolboxName) returns a toolbox which was used to create a button.)
```lua
local Toolbox = plugin:CreateToolbox("Test")
```

and now we'll create a button
(Toolbox:CreateButton(Name, Description, Icon) returns a button)
```lua
local Button = Toolbox:CreateButton("Test", "Just a test.", "rbxassetid://4733890")
```

## How to use
So, we just made a toolbox and a button, but how do we use it? Here we go.

To detect if you clicked the button, use `Button.Click` event.
```lua
Button.Click:Connect(function()
   print("Someone clicked the button!")
end)
```

Now look in the output, it should say:
```lua
Someone clicked the button!
```

# TBA...
If there's any issues that you can't fix, please create an issue.

https://developer.roblox.com/en-us/articles/Intro-to-Plugins

[< Go back to the main page](https://github.com/RocketB0ii/LuaBlox)
