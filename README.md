# Binds mod

This mod allows you to bind any item to a command and use it. 

## How does it work?

Take any item in your hand and type the `/bind` command with your arguments. When you punch with this item, the command will execute automatically.

## Command Usage

### Arguments:

`[reloading]`(Optional) — Cooldown in seconds before the item can be used again. If not specified, defaults to 3 seconds.
`[disposable]` (Optional, 0 or 1) — Set to `1` to make the item single-use. The bind will automatically delete itself after the first successful execution. Defaults to `0` (reusable).
`[tick]` (Optional) — Turns on dynamic targeting. When you punch another player, their nickname is automatically passed as an argument to your command. (Requires `binds` privilege).
`<cmd>` (Required) — The chat command you want to bind (e.g., `say Hello`, `kill`, `grant`). You can write it with or without the leading slash.
`[playertrue]` (Optional)* — Makes the bind global. Other players will be able to use this item and trigger the command. (Requires `binds` privilege).

### Examples:

 `/bind /say Hello` — Simple bind. Reusable, 3 seconds cooldown, prints "Hello" in chat.
 `/bind 5 1 /heal` — Single-use bind with a 5-second cooldown that runs `/heal`.
 `/bind 0 0 tick kill` — Creates a weapon that kills any player you punch instantly with 0 cooldown.
`/bind 10 0 /time day playertrue`


