# GM:SendVerboseCallingCard

Sends a fully customizable calling card to the provided player

(ply, name, card, ctype)

## Arguments
`Player ply` The receiver of the calling card

`string name` The displayed name

`string card` The ID of the calling card

`number ctype = RC_CC_NOTHING` The message of the calling card `globals/RC_CC`

## Example
Sends the world's calling card to the first player
```lua
GM:SendCallingCard(Entity(1), game.GetWorld(), RC_CC_NOTHING)
```