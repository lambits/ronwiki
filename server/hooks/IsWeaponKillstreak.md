# `boolean` IsWeaponKillstreak

Runs when a weapon is picked up and checks if it is a killstreak.

## Arguments
`Player ply` The player picking up the weapon

`Weapon weapon` The weapon in question

## Returns
`boolean` Return true to allow picking up this weapon

## Example
Snippet of code from `sv_modules/sv_loadout.lua`, automatically allows Warzone Parachutes, skydiving and ActMod
```lua
local DefaultWeaponWhitelist = {
    ["aact_weapact"] = true,
    ["voskydiving"] = true,
    ["ventparachute"] = true
}
hook.Add("IsWeaponKillstreak", "roncontroller-allowactmod", function(ply, wep)
    if DefaultWeaponWhitelist[wep:GetClass()] then return true end
end)
```