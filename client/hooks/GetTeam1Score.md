# `number` GetTeam1Score

Used to overwrite the first team's score at the top

## Returns
`number` Team 1's new cosmetic score

## Example
Changes the first team's score to 69
```lua
hook.Add("GetTeam1Score", "reddithumor", function()
    return 69
end)
```