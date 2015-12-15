# electron-ejs-layout

[![npm](https://img.shields.io/npm/v/electron-ejs.svg?style=flat-square)](https://www.npmjs.com/package/electron-ejs)
[![npm](https://img.shields.io/npm/dt/electron-ejs.svg?style=flat-square)](https://www.npmjs.com/package/electron-ejs)

Simple Electron plugin for render EJS templates. It allow you to use `ejs` files in your electron projects and you can define some layouts.


## How to use it

For initialize **electron-ejs** on your project, simply add

```javascript
//In main process.
var electronEjs = require('electron-ejs')(locals);
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

You can publish issues here https://github.com/jpcweb/electron-ejs/issues

## License

**electron-ejs** is under the [MIT](LICENSE) license.
