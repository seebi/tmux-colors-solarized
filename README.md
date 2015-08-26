# Solarize color theme tmux configuration

A tmux solarized theme using Ethan Schoonover’s [Solarized color scheme](http://ethanschoonover.com/solarized).

## Repositories
  * This theme as a single repository: [/seebi/tmux-colors-solarized](https://github.com/seebi/tmux-colors-solarized)
  * The main solarized repository: [/altercation/solarized](https://github.com/altercation/solarized)

## Installation
These config snippets for the terminal multiplexer tmux should be added to your `~/.tmux.conf` configuration file.
This means you have to append the content of e.g. `tmuxcolors-256.conf` to the end of your own config e.g. by using this oneliner (backup you config first!!):

    cat tmuxcolors-256.conf >> ~/.tmux.conf

In most cases, you have to force tmux to assume the terminal supports 256 colours.
For this, start tmux as `tmux -2`.

This color scheme is tested with tmux >= 1.5. tmux 1.1 is reported as not working.

### Installation with [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm)

Add plugin to the list of TPM plugins in `.tmux.conf`:

    set -g @plugin 'seebi/tmux-colors-solarized'

Hit `prefix + I` to fetch the plugin and source it. The plugin should now be working.

3 themes are provided so you can pick and choose via `.tmux.conf` option:

- `set -g @colors-solarized '256'` (the default)
- `set -g @colors-solarized 'dark'`
- `set -g @colors-solarized 'light'`

## Screenshot
Here is a screenshot of a tmux session captured from a gnome-terminal using the [dz-version of the awesome Inconsolata font](http://nodnod.net/2009/feb/12/adding-straight-single-and-double-quotes-inconsola/).

![screenshot](https://github.com/seebi/tmux-colors-solarized/raw/master/tmuxcolors.png)

And another one showing different dircolors from the neighboring [dircolors-solarized](https://github.com/seebi/dircolors-solarized) repository.

![screenshot](https://github.com/seebi/dircolors-solarized/raw/master/img/dircolors.256dark.png)
