# electron-apps [![Build Status](https://travis-ci.org/electron/electron-apps.svg?branch=master)](https://travis-ci.org/electron/electron-apps)

A collection of apps built on Electron. [electron.atom.io/apps](http://electron.atom.io/apps).

## Adding your app

If you have an Electron application you'd like to see added, please
[open a pull request](https://help.github.com/articles/creating-a-pull-request/)!
All that's required is a basic YML file and a PNG icon.

### Using the wizard 🔮

This repository has a CLI wizard much like `npm init` that you can use to generate
a YML datafile for your app. To use the wizard,
[fork and clone this repository](https://help.github.com/articles/fork-a-repo/),
then run:

```sh
npm install && npm run wizard
```

### Adding your app by hand 💪

Another easy way to add a new app is to copy an existing app and edit its metadata.

To do so, create a new directory in the `apps` directory and include a `.yml`
file and `.png` icon file. The directory can only contain numbers,
lowercase letters, and dashes, and the yml and icon files should be named
like so:

```
apps
└── my-cool-app
    ├── my-cool-app-icon.png
    └── my-cool-app.yml
```

YML file rules:

- `name` is required.
- `description` is required.
- `website` is required, and must be a fully-qualified URL.
- `repository` is optional, but must be a fully-qualified URL if provided.
- `keywords` is optional, but should be an array if provided.
- `license` is optional.
- No fields should be left blank.

Icon file rules:

- Must be a `.png`
- Must be a square
- Must be at least 256px by 256px

## Tests

```sh
npm install
npm test
```

## License

MIT
