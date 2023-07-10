# `string` GetTimerText

Used to overwrite the timer's text at the top

## Returns
`string` The new timer text

## Example
Snippet from Demolition's `cl_init.lua`, gets the time from `GAMEMODE.Timer` and shows miliseconds if the timer has less than 30 seconds left
```lua
hook.Add("GetTimerText", "roncontroller-dem-showtimer", function()
    local timernum = math.max(GAMEMODE.Timer - CurTime(), 0)
    local timertext = string.ToMinutesSeconds(timernum)
    if timernum < 30 then
        timertext = string.ToMinutesSecondsMilliseconds(timernum)
    end

    return timertext
end)
```