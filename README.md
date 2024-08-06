# wemcEvent

`wemcEvent` is a Minecraft plugin designed for Spigot and Paper servers. It allows server administrators to broadcast customizable event messages to the entire server.

## Features

- **Broadcast Messages**: Send messages to all players on the server using predefined templates.
- **Customizable Templates**: Define and edit message templates in `messages.yml`.
- **Help Command**: Provides information on available commands.

## Commands

- **/event <template1>**
  - `template1` is editable  
  - Requires permission: `wemcEvent.admin`

- **/wemcevent help**
  - Shows all available commands and their usage.
  - Requires permission: `wemcEvent.admin`

## Configuration

### messages.yml

The `messages.yml` file allows you to define message templates. Here is an example configuration:

```yaml
messages:
  no-permission: "You do not have permission to use this command."
  template-not-found: "Template not found!"

  template1:
    prefix: "<&aWemcEvent&r>"
    message:
      - "--------------------------------"
      - "Template: 1"
      - "&cH&eE&al&5l&1o &fW&bo&lrld"
      - "Whole server can see this"
      - "You can add max 20 lines"
      - "---------------"

  template2:
    prefix: "&r<&c&lServer&r>"
    message:
      - "Hello?"
      - "&cGood &aMorning!"
      - "&k----------"
