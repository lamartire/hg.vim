# hg.vim

<p align="center">
  <img src="./static/intro.jpg" width="450px" />
</p>

## Features

- Dimmed colors for eyes relaxing
- Design on the edge of the light and dark themes
- Minimalistic color palette
- Only important things highlight

![hg preview](./static/preview.jpg)

## Install

### vim

Via `Packer` for `neovim`:

```
use { "lamartire/hg.vim", { rtp = "dist/vim" } }
```

### alacritty

Just insert [`alacritty/hg.yml`](./dist/alacritty/hg.yml) content to your 
`.config/alacritty/alacritty.yml` file.

### tmux

At this moment I'm working on `tpm` plugin, but you can install it manually,
by inserting [`tmux/hg.tmux`](./dist/tmux/hg.tmux) content to your 
`.tmux.conf` file. Then hit `Ctrl+b I` to reload `tmux`.

## Styleguide

All the color tokens are located in `tokens.yml` file. Under the hood, `hg` use
`handlebars` to pass colors to the templates. Explore `src/` directory for examples.

If you want to contribute, please use colors from `tokens.yml` only.

## Build

If you want to contribute or just build your own `hg` option, you should install
`ruby` and run `ruby ./scripts/build.rb`. Then, use files from `dist` directory.

## Credit

Strongly inspired by [alabaster][alabaster].

[alabaster]: https://github.com/tonsky/sublime-scheme-alabaster/
