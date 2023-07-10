# OnPlayerReady

Runs when a player has fully loaded in and can receive net messages

## Arguments
`Player ply` The player who joined

## Example
Snippet of code from Demolition's `init.lua`, sends the time left to the player
```lua
GM.TeamCheckTimer = GM.TeamCheckTimer or 0
hook.Add("OnPlayerReady", "roncontroller-dem-updatetimer", function(ply)
    net.Start("roncontroller-dem-receivetimer")
    net.WriteFloat(GAMEMODE.TeamCheckTimer)
    net.Send(ply)
end)
```