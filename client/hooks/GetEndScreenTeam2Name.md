# `string` GetEndScreenTeam2Name

Used to overwrite the second team's name in the end screen

## Returns
`string` Team 2's new cosmetic name

## Example
Changes the second team's name to "Pee"
```lua
hook.Add("GetEndScreenTeam2Name", "6yohumor", function()
    return "Pee"
end)
```