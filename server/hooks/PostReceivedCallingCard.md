# PostReceivedCallingCard

Runs after a player has received a calling card. This will not run if the calling card was sent using `GM:SendCallingCard` or if `OnSendCallingCard` returned `true`.

## Arguments
`Player ply`
The receiver of the calling card

`Player cardofwho`
The person whose calling card will be displayed

`number ctype`
The type of message what was displayed with the calling card. See `globals/RC_CC`