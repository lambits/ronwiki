# `RC_TYPE`

Used internally in determining the type of weapon

|                        |                                      |
|------------------------|--------------------------------------|
| `RC_TYPE_INVALID`      | The weapon is invalid                |
| `RC_TYPE_PRIMARY`      | The weapon is either in slots 3 or 4 |
| `RC_TYPE_SECONDARY`    | The weapon is either in slots 1 or 2 |
| `RC_TYPE_GRENADE`      | The weapon is either in slots 5 or 6 |
| `RC_TYPE_KILLSTREAK`   | The weapon was given special permissions using the `IsWeaponKillstreak` hook |