# `any` IsSameTeam

Runs to determine if the target ID should show up as friendly or as hostile. Does not run if `TargetIDHidePlayer` returns `true`

## Arguments
`Player ply` The player who is viewing the target (The player we are spectating or us)

`Player target` The target

## Returns
`any` Return a value other than `nil` to change the default behavior

## Example
Shows every player as hostile. Useful for FFA modes
```lua
hook.Add("IsSameTeam", "cod4ffa", function(ply, target)
    return false
end)
```