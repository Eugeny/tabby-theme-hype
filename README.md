# Hype Theme

#### For the Terminus terminal

This is a simple theme that mimicks the Hyper terminal. You can use this plugin as a base to build a theme of your own!

![](http://imgur.com/download/1cEi7ef)

---

## Hacking

Terminus layout is based on Bootstrap 4, so the easiest way is to base the theme on Bootstrap as well.

The styles are located in the [theme.scss](https://github.com/Eugeny/terminus-theme-hype/blob/master/src/theme.scss) file. It starts with a few Bootstrap variable overrides, then Bootstrap itself is included, and then there are some more direct style overrides.

Adjust the theme name and terminal background color in [index.ts](https://github.com/Eugeny/terminus-theme-hype/blob/master/src/index.ts)

Clone this repository and run:

```
npm install
```

Start Webpack in the watch mode:

```
npm run watch
```

and your changes to the styles will be rebuilt automatically.

Meanwhile, start Terminus with this plugin included:

```
TERMINUS_PLUGINS=$(pwd) terminus --debug
```

While Terminus is running, you can reload the plugins by pressing `Ctrl-R` (`Cmd-R` on macOS).

When done, publish your theme to NPM!
