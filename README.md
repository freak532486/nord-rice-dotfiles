# Dotfiles for my i3-nord rice
## Disclaimer
If anything is missing, send me a message. The configurations may change slightly depending on my preferences, however I will not stray from the nord theme.

## Programs
I use the following programs to achieve my desktop:
- i3 (Window Manager)
- picom (Composition Manager, for shadows)
- polybar (Status bar)
- dunst (Notification manager)
- Rofi (Launcher and Power menu)
- [`polybar-spotify-module`](https://github.com/mihirlad55/polybar-spotify-module): You need to install this so that the song currently played in spotify will be displayed correctly.

Not in this repository are:
- GTK-Theme (Look for the *Nordic* theme)
- Icon-Theme (Papyrus with Nordic addon (AUR))
- Firefox-Theme (Nord)
- Konsole-Theme (You guessed it... Nord)

## Fonts
You will need the following fonts:
- Ubuntu Font Family (Especially `Ubuntu Mono`)
- `Iosevka Nerd Font`
- `icomoon-feather` (Icons)

You should be able to get them using your package manager.

## Using these dotfiles
These dotfiles are organized as they are in my `~/.config/`. There are three important scripts, all lying in the polybar folder:

- `config/polybar/mybar/launch.sh`: Launches the bar
- `config/polybar/scripts/launcher.sh`: Opens the launcher (rofi) using the correct theme
- `config/polybar/scripts/powermenu.sh`: Opens the powermenu (rofi) using the correct theme

## End result
Your desktop should look something like this:
![My Desktop](https://i.imgur.com/TR7drrb.png)

I adjusted my wallpaper using GIMP: Create a `.colorscheme` file for nord (or your color theme) and put it into `~/.config/GIMP/<ver>/palettes/`. If you don't know the syntax of a `.colorscheme`, check out some default GIMP palettes . They should be in `/usr/share/gimp/<ver>/palettes/`.

After creating the `.colorscheme`, import an image into GIMP. Select `Image -> Mode -> Indexed...`, choose your palette and uncheck the box below the palette dropdown selection. Finally, enable dithering (except if your chosen image has flat colors, then you might not want dithering). Then click `Convert`. Your image should now consist only of the colors in your `.colorscheme`. To further edit the image, set `Mode` back to `RGB`.

This process will work better on images that are already close to your colorscheme. For *nord*, you want a fairly blue-ish image.

![My Wallpaper](https://i.imgur.com/R45uIQv.jpg)