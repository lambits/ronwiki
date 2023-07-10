# `boolean` OnSendCallingCard

Runs when a player will have a calling card shown clientside.
Only called if the calling card was sent using `GM:SendCallingCard`

## Arguments
`Player ply`
The receiver of the calling card

`Player cardofwho`
The person whose calling card will be displayed

`number ctype = RC_CC_NOTHING`
The type of message to be displayed with the calling card. See `globals/RC_CC`

## Returns
`boolean` Return true to prevent the displaying of the calling card

## Example
Invalidates my hard work and instead displays the nickname of the calling card owner
```lua
hook.Add("OnSendCallingCard", "monster", function(ply, cardofwho, ctype)
    ply:PrintMessage(HUD_PRINTCENTER, cardofwho:Nick())
    return true
end)
```