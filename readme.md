# GMail Background GIF Extension

[template]: https://github.com/fregante/browser-extension-template
[publish-release]: https://addons.mozilla.org/en-US/developers/addon/gmail-background-gif/versions/submit/

Makes animated GIFs as GMail background possible. Add a GIF in a Google Photos album and use it as theme in GMail settings.

Prerequisite: node v18.19.0 and run `npm i`.

## Install for Chrome browsers

To install for Chrome browsers:
- download the source folder
- remove the `browser_specific_settings` attribute of the `manifest.json`
- go to `chrome://extensions/`
- enable developer mode (top right)
- click `Load unpacked` (top left) select the `source` folder

## Try extension with web-ext

In a terminal:
```bash
npm run watch
```

In another terminal:
```bash
web-ext run --firefox="C:\Program Files\Mozilla Firefox\firefox.exe"
```

## Quick build - Release guide

```bash
npm run build
web-ext build
```

The built extension is in `web-ext-artifacts`.

Publish it by hand on [this page](publish-release).

## Template

The template used for this extension: [browser-extension-template](template).
