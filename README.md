# marp-slide-deck-template

> *Credit goes to [Yuki Hattori](https://github.com/yhatt) for saving me a lot of time so I can focus on putting content together. Cut of [yhatt/marp-cli-example](https://github.com/yhatt/marp-cli-example) with the intent of simplyfing Yuki's work for my own personal use.*

## Slide Deck

> <img src="https://icongr.am/octicons/mark-github.svg" width="24" height="24" valign="bottom" /> [GitHub Pages](https://ve2caz.github.io/marp-slide-deck-template)

## Remotely Access Code

> [![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/ve2caz/marp-slide-deck-template)

### Background

For Marp slide deck features, please see the documentation of [Marpit Markdown](https://marpit.marp.app/markdown), [the features of Marp Core](https://github.com/marp-team/marp-core#features), and the default example in [`SLIDE-DECK.md`](https://raw.githubusercontent.com/ve2caz/marp-cli-example/master/SLIDE-DECK.md) for .

You have to install [Node.js](https://nodejs.org/) and run `npm i` at first if you want to write slide deck with [Marp CLI].

## Usage

### Create new slide deck

[![](https://img.shields.io/badge/-Use%20this%20template-brightgreen?style=for-the-badge&logo=github)](https://github.com/ve2caz/marp-slide-deck-template/generate)

Then [enable GitHub Pages using `gh-pages` branch](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) from **Settings** tab.

### Edit deck

Just edit **[`SLIDE-DECK.md`](./SLIDE-DECK.md)**!

#### Preview deck

**[Marp for VS Code]** extension is the best partner for writing Marp slide deck with live preview.

<p align="center">
  <a href="https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode">
    <img src="https://raw.githubusercontent.com/marp-team/marp-vscode/master/docs/screenshot.png" width="500" />
  </a>
</p>

**You can try edit and preview on the web now!** Open https://github.dev/yhatt/marp-cli-example/blob/master/SLIDE-DECK.md or hit <kbd>.</kbd> key on this repository, and install [Marp for VS Code] extension.

[Marp for VS Code]: https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode

#### Preview via CLI

```zsh
npm run start
```

It will be opened preview window via installed Google Chrome, and track change of `SLIDE-DECK.md`.

### Assets and themes

- `assets` directory can put your assets for using in the deck. (e.g. Image resources)
- `themes` directory can put [custom theme CSS](https://marpit.marp.app/theme-css). To use in the deck, please change `theme` global directive.

### Build deck via CLI

```zsh
npm run build
```

The built assets will output to `dist` folder.

#### Build per assets

```zsh
npm run deck      # Output static HTML to dist/index.html
npm run og-image  # Output image for Open Graph to dist/og-image.jpg
```

## LICENSE

[UNLICENSE](/LICENSE)
