# Canadian Multilingual Standard keyboard layout for Linux console

This adds the Canadian Multilingual Standard keyboard layout to the Linux
console.

For reference the layout is based on the screenshot below, from the Gnome
keyboard settings. Duplicates have been removed, with a preference for the
positions specified in the standard (`¬`, `{`, `}`, `°`).

Note that this layout differs from the standard and the Windows layout,
particularly on the `3`, `4`, and `5` keys.

![](gnome-cms.png)

The file should be copied into `/usr/share/kbd/keymaps/i386/qwerty` or
`/usr/share/keymaps/i386/qwerty` depending on your distro. On Debian you might
need the `console-data` package.

Then, edit `/etc/vconsole.conf` as follows:

    KEYMAP=ca
    FONT=iso01.16
