# `string` GetEndScreenTeam1Score

Used to overwrite the first team's score in the end screen

## Returns
`string` Team 1's new cosmetic score

## Example
Changes the first team's score to -3.1415926
```lua
hook.Add("GetEndScreenTeam1Score", "negativepi", function()
    return -3.1415926
end)
```