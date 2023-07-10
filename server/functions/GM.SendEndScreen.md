# GM:SendEndScreen

Updates the information displayed by the end screen to the provided player

## Arguments
`Player ply` The receiver of the updated end screen info

`number winner` The winning team, the team color will be displayed as a gradient

`number state` The state of the end screen. See `globals/RC_ES`

## Example
Tells the first player that BLUFOR has won and that they have also won
```lua
GM:SendEndScreen(Entity(1), TEAM_BLUFOR, RC_ES_WIN)
```