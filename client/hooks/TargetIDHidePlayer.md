# `boolean` TargetIDHidePlayer

Runs to prevent the default RONController TargetID from showing up per target

## Arguments
`Player ply` The player who is viewing the target (The player we are spectating or us)

`Player target` The target

## Returns
`boolean` Return `true` to hide the target ID

## Example
Hides garry's target ID
```lua
hook.Add("TargetIDHidePlayer", "realgarry", function(ply, target)
    if target:SteamID() == "STEAM_0:1:7099" then return true end
end)
```