# [Catena](https://github.com/alysoid/catena) - Locale Ansible Role

Ansible role to Manage locales and virtual console keymap via systemd.

## Role default variables

| Variable           | Default     | Info
| ------------------ | ----------- | --------------------------------------
| `keymap`           | us          | Used by localectl set-keymap
| `locale`           | en_US.UTF-8 | Used by localectl set-locale LANG=
| `language`         | en_US.UTF-8 | Used by localectl set-locale LANGUAGE=

### `locale`

Sets the default `LANG` environment variable to specify the language on a GNU+Linux system. It's used to print out messages in the chosen language. 

### `language`

Sets the `LANGUAGE` environment variable to specify the order of the languages to be used on a GNU+Linux system. When a translation for the preferred locale is unavailable, the next fallback language is used to display messages. This allow users to specify a list of preferred locales that will be used in that order.
