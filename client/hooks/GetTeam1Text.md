# `string` GetTeam1Text

Used to overwrite the first team's text at the top

## Returns
`string` Team 1's new cosmetic name

## Example
Changes the first team's name to "Poop"
```lua
hook.Add("GetTeam1Text", "12yohumor", function()
    return "Poop"
end)
```