# fireclickdetector guide

```lua
fireclickdetector(detector [, player])
```

detector: The ClickDetector instance you want to activate.

player: LocalPlayer

# Notes:

- The object the ClickDetector is attached to must be clickable (within range if game uses distance checks).

- You can fire the click detector multiple times programmatically.

# Example

- Simulating clicking an example ClickDetector:

```lua
local player = game.Players.LocalPlayer
local detector = workspace.Example.ClickDetector

fireclickdetector(detector, player)
```
