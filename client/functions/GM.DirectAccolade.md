# `number` GM:DirectAccolade

Displays a *Call of Duty: Modern Warfare 2*-styled accolade at the top of the screen with no delay

## Arguments
`string title = ""` The title of the accolade

`string description = ""` The description of the accolade

`number fadein = 0.125` The fade in duration of the accolade

`number duration = 2.5` The duration of the accolade

`number fadeout = 0.125` The fade out duration of the accolade

`IMaterial image = nil` The icon displayed by the accolade, `nil` represents no image

`string sfx = ""` Sound played by the accolade

`boolean scale` Whether the accolade will change sizes during the fade in and fade out processes

## Returns
`number` The accolade's total display time without the fade out time

## Example
Displays an accolade that says "**Headshot! (+50)**", playing the Call of Duty 4 Last Stand sound
```lua
GM:DirectAccolade("Headshot!", "(+50)", 0.125, 2.5, 0.125, Material("icon16/user.png"), Sound("RONController.UI.LastStand"), true)
```