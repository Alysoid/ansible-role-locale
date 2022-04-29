# [Catena](https://github.com/alysoid/catena) Ansible Role: locale

Ansible role to manage locales and virtual console keymap via systemd.

## Role default variables

| Variable   | Default          | Info                                     |
| ---------- | ---------------- | ---------------------------------------- |
| `keymap`   | `us`             | Used by `localectl set-keymap`           |
| `lang`     | `en_US.UTF-8`    | Used by `localectl set-locale LANG=`     |
| `language` | `en_US:en_GB:en` | Used by `localectl set-locale LANGUAGE=` |

### `keymap`

[Keyboard mappings](https://wiki.archlinux.org/title/Linux_console/Keyboard_configuration) (keymaps) for the Linux console.

For a list of all available keymaps, use the command `localectl list-keymaps`

### `lang`

[Default locale](https://wiki.archlinux.org/title/locale#LANG:_default_locale) with `LANG` environment variable to specify the language on a GNU+Linux system. Set all the `LC_*` variables that are not explicitly set. It's used to print out messages in the chosen language.

### `language`

[Fallback locale](https://wiki.archlinux.org/title/locale#LANGUAGE:_fallback_locales) with `LANGUAGE` environment variable. Specify the order of languages when a translation is unavailable. It is a list of preferred locales that will be used in that order.
