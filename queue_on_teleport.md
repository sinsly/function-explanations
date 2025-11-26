# queue_on_teleport guide

- queue_on_teleport is a function that allows you to queue a script to run automatically after a player teleports to a new place in Roblox.

## Syntax

```lua
queue_on_teleport(scriptOrString)
```

- scriptOrString: The Lua code (as a string) or the path to a script file you want to execute after teleport.

# Basic Example

- Queue a simple print statement to run after teleport:

```lua
queue_on_teleport([[
print("Teleported")
]])
```

- Once the player teleports, this message will print in the output.
- I suggest running this through a loadstring script as an auto exeucte add-on / alternative without needing to add it to your folder.
