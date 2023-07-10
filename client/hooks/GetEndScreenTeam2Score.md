# `string` GetEndScreenTeam2Score

Used to overwrite the second team's score in the end screen

## Returns
`string` Team 2's new cosmetic score

## Example
Changes the first team's score to 3.1415926
```lua
hook.Add("GetEndScreenTeam2Score", "pi", function()
    return 3.1415926
end)
```