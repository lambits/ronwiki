# `string` GetTeam2Text

Used to overwrite the second team's text at the top

## Returns
`string` Team 2's new cosmetic name

## Example
Changes the second team's name to "Fart"
```lua
hook.Add("GetTeam2Text", "9yohumor", function()
    return "Fart"
end)
```