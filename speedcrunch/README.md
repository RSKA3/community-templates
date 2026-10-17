# Noctalia SpeedCrunch Template

A [Noctalia](https://github.com/noctalia-dev/noctalia-shell) user template that generates a [SpeedCrunch](https://github.com/heldercorreia/speedcrunch) theme from your current Noctalia colors.

## Files

| File | Purpose |
| --- | --- |
| `speedcrunch.json` | The template. |
| `speedcrunch.toml` | The Noctalia config snippet that registers the template. |

## Setup

1. Copy `speedcrunch.json` somewhere permanent, for example `~/.config/noctalia/templates/speedcrunch.json`.

2. Add the contents of `speedcrunch.toml` to your Noctalia user templates config and point `input_path` at the template:

   ```toml
   [theme.templates.user.speedcrunch]
   input_path  = "~/.config/noctalia/templates/speedcrunch.json"
   output_path = "~/.local/share/SpeedCrunch/color-schemes/Noctalia.json"
   ```

   The output must go straight into SpeedCrunch's `color-schemes` folder.

3. Trigger a theme regeneration in Noctalia (for example by changing the wallpaper or color scheme).

4. In SpeedCrunch, open the color scheme settings: 
   ```
   Settings -> Appearance -> Theme -> Import Theme -> ~/.local/share/SpeedCrunch/color-schemes/Noctalia.json.
   ```