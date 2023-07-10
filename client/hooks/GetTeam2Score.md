# `number` GetTeam2Score

Used to overwrite the second team's score at the top

## Returns
`number` Team 2's new cosmetic score

## Example
Changes the second team's score to 420
```lua
hook.Add("GetTeam1Score", "alsoreddithumor", function()
    return 420
end)
```