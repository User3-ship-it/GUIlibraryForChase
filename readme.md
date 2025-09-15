# Flip's UI library
so yeah this is just an simple but good ui library for roblox

i dont really know what to say here so yeah

## How to use

First, Start by putting this line of code in ur executor

```bash
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/User3-ship-it/GUIlibraryForChase/refs/heads/main/FlipOne"))()
library.TransitionSpeed = 0.19
library.WaitForNext = 0.055
library.TransitionBack = 0.01
```
This is just to reference the system so u can use its functions later

To make a new Library GUI do this after referencing library

```python
local engine = library:New("Flipped")
```
This makes a new thingy idk

To make a tab just do:

```bash
local tab1 = engine:CreateTab("Main")
```
### --Elements--

Currently, u can only make Dropdowns,Buttons,Toggles and Sliders :( but soon i will make more options

lets say u made ur tab, Now lets give it some elements!

```bash
tab1:NewButton("Press me!", function()
    print("hello iam a button!")
end)
```

this OBIOUSLY makes a button, you can also do:

```bash
local dropdown = tab1:NewDropdown("Single",  {"Option2","Option1"}, "Name")
```
if u want to get the current selected values from a dropdown on a diferent part of the code, just do:

```bash
dropdown:GetSelected()
```

There are 2 dropdown types: Single and Multiple

To make a slider, do this:

```bash
tab1:NewSlider("Slider", 0, 100, 16, function(v)
    print(v)
end)
```

v is the current value of the slider, the Second argument is the Minimum Value, the Third argument is the Max. Value and the Fourth value is the starting value

And finally,
To make a toggle, this is what u do:

```bash
tab1:NewToggle("My Toggle", function(v)
    print(v)
end)
```

i really dont know how to explain how to use this, my bad if my explaination was absolute TRASH

