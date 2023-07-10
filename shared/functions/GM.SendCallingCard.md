# GM:SendCallingCard

Sends another player's calling card to the provided player

## Arguments
`Player ply` The receiver of the calling card

`Entity cardofwho` The owner of the calling card. The calling card will be random if this entity is not a player

`number ctype = RC_CC_NOTHING` The message of the calling card. See `globals/RC_CC`

## Example
Sends the world's calling card to the first player
```lua
GM:SendCallingCard(Entity(1), game.GetWorld(), RC_CC_NOTHING)
```