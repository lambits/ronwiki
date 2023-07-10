# AddExtraCallingCards

Runs when the calling card table is initialized, allows for adding custom calling cards

## Example
Replaces "National: Poland"'s image with with "Poland Special"'s image and changes its name.
```lua
hook.Add("AddExtraCallingCards", "nonewstuffhuh", function()
    GAMEMODE.CallingCards["national-pl"] = {
        name = "International: Poland",
        image = "roncontroller/callingcards/rin-national-pl.jpg"
    }
end)
```