# WemcEvent Plugins

**Version:** 0.6.1 [ (Download) ](https://github.com/wejkeyy/wemcEvent/raw/main/plugin_versions/Event_0.6.1.jar)<br>
Spigot: [here](https://www.spigotmc.org/resources/wemcevent.118712/)


## Description

`wemcEvent` is a simple Minecraft plugin for Spigot/Paper that allows server administrators to broadcast event messages to all players. Administrators can send other things other than events but remember that command is `/event`

## Features

- Broadcast messages to all players on the server.
- Messages and prefixes are customizable via `messages.yml`.
- Supports up to 20 lines per message template.
- That `template1` or `template2` can be added/renamed/removed

## Commands

- `/event <templateName>`

## Permissions

- `wemcEvent.admin`: Required to use the `/event` command. Or: **OP**

## Configuration

### `messages.yml`

Define message templates in `messages.yml`:

```yaml
template1:
  prefix: "&aWemcEvent" # Prefix in the chat
  message:
    - "--------------------------------"
    - "Template: 1"
    - "&cH&eE&al&5l&1o &fW&bo&lrld"
    - "Whole server can see this"
    - "You can add max 20 lines"
    - "---------------"

template2:
  prefix: "&r<&c&lServer&r>" # Prefix in the chat
  message:
    - "Hello?"
    - "&cGood &aMorning!"
    - "&k----------"
