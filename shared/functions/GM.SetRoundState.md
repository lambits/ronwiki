# GM:SetRoundState

Changes the round state. Running this clientside only changes the local state

## Arguments
`number state` The new round state. See `globals/ROUND`

## Example
Sets the round state to `ROUND_PROGRESS`
```lua
GM:SetRoundState(ROUND_PROGRESS)
```