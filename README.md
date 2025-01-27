# Return To Same Place

This script allows you to save your location and teleport to it across games.

### Warning: It is not safe for games with anti tp cheats, Your executor need writefile/readfile functions.

## Main Source
#### After executing, Rejoin for the script to work.
```lua
-- // [Made by MommyW6] [Full docs at: https://github.com/MommyW6/Return/blob/home/README.md]
loadstring(game:HttpGet("https://raw.githubusercontent.com/MommyW6/Return/home/SameOldPlace"))();

local Time = 3 -- // will save your position every 3 seconds!~
getgenv().LoadPosition("Teleport")();
while true do task.wait(Time)pcall(function()getgenv().SavePosition()end)end;
```

## Functions:
#### Use these if you want? Idk...
```
getgenv().LoadPosition("Teleport")(); -- // Will load your position. (Teleport method)
getgenv().LoadPosition("Tween")(50); -- // Will load your position. (Tween method)
```

```
getgenv().SavePosition(); -- // Will save your position.
```

## Reset Location:
#### Only use it when the loop is not running.
For the game you are in:
```lua
local file = "ReturnFolder".."/Return - "..game.PlaceId;if isfile(file) then delfile(file) end -- // Deletes your file (In the game you are in);
```
For all the games you are were in:
```lua
local folder = "ReturnFolder";if isfolder(folder) then delfolder(folder) end -- // Deletes your folder (All the games you were in);
```
-----------------------------------------------
#### Made by MommyW6
