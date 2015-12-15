# electron-ejs-layout

[![npm](https://img.shields.io/npm/v/electron-ejs-layout.svg?style=flat-square)](https://www.npmjs.com/package/electron-ejs-layout)
[![npm](https://img.shields.io/npm/dt/electron-ejs-layout.svg?style=flat-square)](https://www.npmjs.com/package/electron-ejs-layout)

Simple Electron plugin for render EJS templates. It allow you to use `ejs` files in your electron projects and you can define some layouts.


## How to use it

Install with npm

```sh
npm install electron-ejs-layout
```

For initialize **electron-ejs-layout** on your project, simply add

```javascript
//In main process.
var electronEjs = require('electron-ejs-layout')(locals);
conf = {
    layoutViewPath: __dirname+'/views/'
};
...
//You have to define layoutFile
conf.layoutFile = 'layout.ejs';
mainWindow.loadURL('file://'+__dirname+'/views/main/main.ejs');
```

Where `locals` is an object where each key is used as a variable in your template.


## Issues

You can publish issues here https://github.com/jpcweb/electron-ejs-layout/issues

## License

**electron-ejs-layout** is under the [MIT](LICENSE) license.
