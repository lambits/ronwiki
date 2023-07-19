# `boolean` ClassPlayerDeath

Called from the player's class on death

## Arguments
`Player victim` The player who died

`Entity inflictor` Item used to kill the victim

`Entity attacker` Player or entity that killed the victim

## Returns
`boolean` Return `true` to stop the deathcam and freezecam

## Example
Prevents the default death camera behavior
```lua
hook.Add("ClassPlayerDeath", "stopsourcecam", function(victim, inflictor, attacker)
    return true
end)
```