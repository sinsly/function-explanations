# fireproximityprompt guide

```lua
fireproximityprompt(prompt [, player, holdDuration])
```

- prompt: The ProximityPrompt instance you want to activate.

- player (optional): The player who is “interacting.” Defaults to LocalPlayer.

- holdDuration (optional): Duration to hold the prompt for HoldDuration prompts.

## Notes:

If the prompt has a HoldDuration, you can simulate holding it by passing the duration in seconds.
Or you can define the prompt parent and change the HoldDuration.
```lua
prompt.HoldDuration = 0
```

## Example

Simulating pressing a door prompt:

```lua
local player = game.Players.LocalPlayer
local doorPrompt = workspace.Door.ProximityPrompt

fireproximityprompt(doorPrompt, player)
```
