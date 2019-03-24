# firefox-local-newtab-page
Loads a page from the extension's own files when a new tab is opened.
If you put other files, like css, along with your page, it will successfully reference it as long as it uses relative paths.

Extensions on the Firefox marketplace are unable to set new tab pages to a local page because they are not part of the extension itself and Firefox sandboxes extensions' files. This is an unpackaged extension so you can put your own `homepage.html` in the `newtab-page` directory so it will load.

To load the extension, I reccommend you put the source code in some directory, go to `about:debugging`, enable temporary add-ons, and load the extension by opening `manifest.json`. This lets you replace or modify the homepage whenever you want without even having to reload the extension in Firefox.

Optionally you *could* sign the extension with the Add-On Developer Hub and load it like a regular XPI, since I tested it and it works.
