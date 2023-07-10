# `string` GetEndScreenTeam1Name

Used to overwrite the first team's name in the end screen

## Returns
`string` Team 1's new cosmetic name

## Example
Changes the first team's name to "Poop"
```lua
hook.Add("GetEndScreenTeam1Name", "12yohumor", function()
    return "Poop"
end)
```