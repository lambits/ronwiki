# GM:SendMOTD

Sends the provided HTML to a player

## Arguments
`Player ply` The receiver of the MOTD

`string HTML` The HTML to be sent to the player. It will be compressed

## Example
Sends a player a nice MOTD when they join
```lua
hook.Add("OnPlayerReady", "sneedmotd", function(ply)
    GAMEMODE:SendMOTD(ply, "<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>")
end)
```