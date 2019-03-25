# firefox-local-newtab-page
Loads a page from the extension's own files when a new tab is opened.
If you put other files, like css, along with your page, it will successfully reference it as long as it uses relative paths.

Extensions on the Firefox marketplace are unable to set new tab pages to a local page because they are not part of the extension itself and Firefox sandboxes extensions' files. This is an unpackaged extension so you can put your own `homepage.html` in the `newtab-page` directory so it will load.

To load the extension, you should put the extension (including your new tab page) in a zip file and sign it with Mozilla Add-on Developer Hub. Then you can use the "Install Add-ons from file" option in `about:addons` to load the XPI.
