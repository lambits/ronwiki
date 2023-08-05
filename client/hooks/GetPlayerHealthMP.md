# `number` `boolean` GetPlayerHealthMP

The health bar's multiplier to be displayed in the HUD. This value is not clamped by default, therefore it can go out of its desired space

## Arguments
`Player ply` The player currently being spectated, or the local player

## Returns
`number` Fraction of the bar to be displayed. 1 or 0 hides the bar

`boolean` Whether or not the health is at a critical level. Returning `true` causes the health bar to pulse red