# RONControllerLoadout

Called from the player class's loadout function as a replacement.

## Arguments
`Player ply` The player who the weapons are being given to

## Example
Snippet from Demolition's `init.lua`, gives any member of OPFOR a C4
```lua
hook.Add("RONControllerLoadout", "roncontroller-dem-givec4", function(ply)
    if ply:Team() == TEAM_OPFOR then ply:Give("weapon_roncontroller_c4") end
end)
```