# `boolean` DamageViewPunch

Runs when a player will get viewpunch from taking damage

## Arguments
`Player ply`
The player taking damage

`Player attacker`
The player who dealt the damage

`number health`
The remaining health of `ply`

`number damage`
The amount of damage dealt to `ply`

## Returns
`boolean` Return true to prevent viewpunch from being applied

## Example
Makes the viewpunch worse by overwriting the behavior
```lua
hook.Add("DamageViewPunch", "makeitworse", function(ply, attacker, health, damage)
    ply:SetViewPunchVelocity(Angle(damage * -3, 0, 0))
    return true
end)
```