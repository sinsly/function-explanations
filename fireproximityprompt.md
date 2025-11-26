# fireproximityprompt guide

```lua
fireproximityprompt(prompt [, player, holdDuration])
```

- prompt: The ProximityPrompt instance you want to activate.

- player: LocalPlayer.

- holdDuration (optional): Duration to hold the prompt for HoldDuration prompts.

## Notes:

Distance can prevent the firing of Proximity Prompts.
You can define the prompt parent and change the HoldDuration time.
If the prompt has a HoldDuration, you can simulate holding it by passing the duration in seconds.

```lua
prompt.HoldDuration = 0
```

## Example

Simulating pressing an example prompt:

```lua
local player = game.Players.LocalPlayer
local prompt = workspace.Example.ProximityPrompt

fireproximityprompt(prompt, player)
```
