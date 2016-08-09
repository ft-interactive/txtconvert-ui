# Text Spreadsheet Converter
## 2016 Ændrew Rininsland

This is a simple Electron app that parses through the text spreadsheets used by the Financial Times
stats team and returns both a clean CSV and a metadata file. The metadata is generated via
lines starting with `&`.

The first "comment" line is generally the header row. This is added to the output as such.

The first field in the header row is often omitted; this gets re-added as "date".

The underlying processing lib is [ft-interactive/txtconverter][1].


## Dev

```
$ npm install
```

### Run

```
$ npm start
```

### Build

```
$ npm run build
```

Builds the app for OS X, Linux, and Windows, using [electron-packager](https://github.com/electron-userland/electron-packager).


## License

MIT © [Ændrew Rininsland](http://ig.ft.com)

[1]: https://github.com/ft-interactive/txtconverter
