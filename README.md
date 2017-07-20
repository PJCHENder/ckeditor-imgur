# CKEditor Plugin with imgur

This is a plugin for CKEditor to upload images directly to imgur through ckeditor. The plugin is forked from [ckeditor-imgur](https://github.com/yfxie/ckeditor-imgur) which was built by [Yi Feng Xie](https://github.com/yfxie). The original plugin do not need access token of imgur, therefore every image uploaded is anonymous. In the plugin, we modify a little code to upload images with access token.

First set the parameters below in `config.js`:

```javascript
// ./ckeditor/plugins/config.js
config.extraPlugins = 'imgur';
config.imgurClientID = 'CLIENT_ID';
config.imgurClientSecret = 'CLIENT_SECRETE';
config.imgurRefreshToken = 'REFRESH_TOKEN';
```

Move all the plugin files into `./ckeditor/plugins/imgur`.

