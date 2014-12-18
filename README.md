# qlImageSize

This is a **QuickLook** plugin for OS X *10.8+* to display the dimensions of an image and its file size in the title bar.

![qlImageSize preview window](http://static.whine.fr/images/2014/qlimagesize1.jpg)

This plugin can also preview and generate Finder thumbnails for unsupported images formats like :

- [bpg](http://bellard.org/bpg/ "bpg")
- [Portable Pixmap](http://en.wikipedia.org/wiki/Netpbm_format "Netpbm")
- [WebP](https://developers.google.com/speed/webp/ "WebP")

![qlImageSize thumbnails generation](http://static.whine.fr/images/2014/qlimagesize3.jpg)

![qlImageSize WebP and PPM preview](http://static.whine.fr/images/2014/qlimagesize2.jpg)

If you are a **Pixelmator** user, its own QuickLook plugin might get in the way when previewing **WebP** files. To fix this you need to edit the file `/Applications/Pixelmator.app/Contents/Library/QuickLook/PixelmatorLook.qlgenerator/Contents/Info.plist` and remove the dict entry that handles **webp**.


### Installation

Download the plugin [here](http://repo.whine.fr/qlImageSize.qlgenerator-10.8.zip "qlImageSize for 10.8+").

Unzip it, and place it in `/Library/QuickLook` or `~/Library/QuickLook`.

You will need to restart the *QuickLook daemon* by running these commands in your Terminal :

	qlmanage -r
	qlmanage -r cache


### License

***qlImageSize*** is released under the *Simplified BSD license*, see **LICENSE**.

Blog : [Cocoa in the Shell](http://cocoaintheshell.com "Cocoa in the Shell")

Twitter : [@Nyx0uf](https://twitter.com/Nyx0uf "Nyx0uf on Twitter")

---

### About Mavericks (OS X 10.9)

**qlImageSize** doesn't fully work on 10.9. By fully, I mean it works for certain types of images like *tga*, *bmp*, *psd*, *tif* but not for the common ones *jpg*, *png*, *gif*.

It is a known bug in the OS and I can't do anything about it, Apple never fixed it and won't. The best way is to update to this ugly as fuck 10.10, how sad.

For more informations, see [issue 4](https://github.com/Nyx0uf/qlImageSize/issues/4 "issue 4").
