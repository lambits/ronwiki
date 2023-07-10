# `number` GM:DirectCardSlide

Displays a *Call of Duty: Modern Warfare 3*-styled card slide in the top-right corner of the screen

## Arguments
(name, action, pteam, fadein, duration, fadeout, sfx)
`string name = ""` The name of the player

`string action = ""` The message below the name

`number pteam = 1001` The team of which color will be used for the name

`number fadein = 0.125` The fade in duration of the accolade

`number duration = 2.5` The duration of the accolade

`number fadeout = 0.125` The fade out duration of the accolade

`string sfx = ""` Sound played by the card slide

## Returns
`number` The card slide's total display time without the fade out time

## Example
Displays a card slide that says the first player's name and says "**Humiliation!**"
```lua
GM:DirectCardSlide(Entity(1):Nick(), "Humiliation!", Entity(1):Team(), 0.125, 2.5, 0.125, Sound("RONController.UI.CardSlide"))
```