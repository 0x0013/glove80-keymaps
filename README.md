# "Glorious Engrammer" keymaps for MoErgo Glove80

These are [my Glove80][1] keymaps featuring the [Engram][2]([mer][3]) 
layouts with [Miryoku][4] style layers and [home row mods][5].

>![Photograph of my Glove80 with Engrammer layout](https://raw.githubusercontent.com/sunaku/sunaku.github.io/master/moergo-glove80-keyboard-photograph.jpg)

[1]: https://sunaku.github.io/moergo-glove80-keyboard.html
[2]: https://sunaku.github.io/engram-keyboard-layout.html
[3]: https://sunaku.github.io/engrammer-keyboard-layout.html
[4]: https://github.com/manna-harbour/miryoku
[5]: https://sunaku.github.io/home-row-mods.html

## Legend

See [interactive layer map][6] for overview and documentation.  

NOTE: This is also available as a [printable PDF document][7].

[6]: https://sunaku.github.io/moergo-glove80-keyboard.html#layers
[7]: https://sunaku.github.io/moergo-glove80-keyboard-layers.pdf

## Keymaps

- for Engrammer layout: https://my.glove80.com/#/layout/user/a32711f5-014e-4581-b1e9-1351851f5559
- for Arno's Engram 2.0: https://my.glove80.com/#/layout/user/96c41146-ce0f-4776-bf54-f53f38718939

## Installing

Refer to the handy [Quickstart Guide] for a step-by-step tutorial with screenshots!

[Quickstart Guide]: https://github.com/sunaku/glove80-keymaps/wiki/Quickstart-Guide

### Flashing

- For the initial flash, use the "bootloader mass storage device mode" method
(see page 31 in the [Glove80 User Guide]).

- If you're installing a different firmware version compared to what your
keyboard currently has, then ⚠️ **after flashing both halves** ⚠️ perform a
*configuration factory reset* on both halves (see page 41 in the [Glove80 User
Guide]) and then toggle the per-key RGB effects first on and then off. ⚡  This
allows the newly installed firmware to take full effect. 💯

[Glove80 User Guide]: https://www.moergo.com/files/glove80-user-guide.pdf

## Upgrading

- Copy the ZMK snippet from the "Custom Defined Behaviors" text box in either
keymap linked above and paste into yours.  The contents of that text box are
also available in the `*.dtsi` files provided in this Git repository.

- You can diff and copy changes between a JSON export of your keymap (via
"Advanced Settings" > "Enable local config" then go back to "Edit" and click
"Download") and the `*.json` files provided in this Git repository.

## Customizing

You can customize the preset characters in the Emoji and World layers by
editing their respective YAML source files in this repository.  Afterwards, 
run the `rake` command to regenerate the "Custom Defined Behaviors" snippet.

To install the prerequisite software for `rake` on a Debian GNU/Linux system:

    apt install ruby rake

### Fine-tuning the timing

Activate the typing layer, launch the [QMK Configurator's testing tool](
https://config.qmk.fm/#/test ), and then pretend to use home row mods. Note the
timing and duration of keystrokes reported by the tool and then use them to
adjust the `#define` time thresholds in the "Custom Defined Behaviors" snippet.

## Discussion

See ["Glorious Engrammer" on Discord][7] for discussion & updates.

[7]: https://discord.com/channels/877392805654306816/1111469812850380831

## License

[Spare A Life]: https://sunaku.github.io/vegan-for-life.html
> Like my work? 👍 Please [spare a life] today as thanks! 🐄🐖🐑🐔🐣🐟✨🙊✌  
> Why? For 💕 ethics, the 🌎 environment, and 💪 health; see link above. 🙇

(the ISC license)

Copyright 2023 Suraj N. Kurapati <https://github.com/sunaku>

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
