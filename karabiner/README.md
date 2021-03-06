# Karabiner-Elements

A powerful and stable keyboard customizer for OS X.

## Installation

For macOS Sierra see https://github.com/tekezo/Karabiner-Elements
For OS X 10.11, 10.10, 10.9 see https://pqrs.org/osx/karabiner/

## Karabiner-Elements (for MacOS Sierra)

Not much of documentation right now, make sure to view `karabiner.json`.

## Karabiner (Legacy)

Everything is inside the [./legacy](./legacy) directory:

### Custom Options (private.xml)

You can create your own custom options that will appear within Karabiner.
These options won't activate until you enable them in the settings menu.

```sh
cd "~/Library/Application Support/Karabiner"
ln -sfv ~/.config/karabiner/legacy/private.xml
/Applications/Karabiner.app/Contents/Library/bin/karabiner reloadxml
```

### Restore Keyboard Settings

You can import stored settings that will automatically select saved options:

- [Truly Ergonomic Keyboard]: `sh ~/.config/karabiner/legacy/import-teck.sh`
- [MacBook] and [Apple Keyboards]: `sh ~/.config/karabiner/legacy/import-macbook.sh`

### Backup Keyboard Settings

Karabiner features a command-line tool that can help:

```sh
/Applications/Karabiner.app/Contents/Library/bin/karabiner export > import.sh
chmod ug+x import.sh
```

Now all you need to do is run `import.sh` to restore your saved settings.

### See Also

- Documentation: https://pqrs.org/osx/karabiner/document.html.en
- Custom options: https://pqrs.org/osx/karabiner/document.html.en#privatexml

[Karabiner]: https://pqrs.org/osx/karabiner/
[Karabiner-Elements]: https://github.com/tekezo/Karabiner-Elements
[Truly Ergonomic Keyboard]: https://www.trulyergonomic.com/
[MacBook]: https://www.apple.com/macbook/design/
[Apple Keyboards]: http://store.apple.com/us/mac/mac-accessories/mice-keyboards
