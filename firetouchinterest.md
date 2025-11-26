# firetouchinterest guide

```lua
firetouchinterest(part1, part2, touchType)
```

part1: The first BasePart (e.g., your character's part like HumanoidRootPart).

part2: The second BasePart (e.g., an in-game item or part).

touchType: Number representing the action:

0 → touch (begin touching)

1 → untouch (stop touching)

## Notes:

part1 is typically the part you control.

part2 is the target part you want to trigger .Touched on.

Using 0 followed by 1 simulates a complete touch.

## Basic Example

Simulating example player touch connect:

```lua
local player = game.Players.LocalPlayer
local hrp = player.Character.HumanoidRootPart
local example = workspace.ExampleTarget

firetouchinterest(hrp, exampl, 0)
firetouchinterest(hrp, example, 1)
```

This triggers the example’s .Touched event as if the player actually walked into it.

Always use 0 before 1. Omitting the untouch may cause unexpected behavior.

Can be combined with RunService.RenderStepped or loops for automation.
