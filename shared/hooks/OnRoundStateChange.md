# OnRoundStateChange

Runs when the round state was changed

## Arguments
`number oldstate` The old round state. See `globals/ROUND`

`number newstate` The updated round state

## Example
Plays Brane Scane from Half-Life 2 clientside if the round is now over and kills every human player serverside
```lua
hook.Add("OnRoundStateChange", "branescan", function(oldstate, newstate)
    if newstate ~= ROUND_OVER then return end

    if CLIENT then surface.PlaySound("music/hl2_song31.mp3") end

    if SERVER then for _, ply in ipairs(player.GetHumans()) do
        ply:Kill() end
    end
end)
```