# Photo Library for Windows

Your photos and videos, gathered in one place on your own computer. Photo Library finds the people in
them, clears out the clutter, and helps you share the best ones. Nothing is uploaded.

**[Download the installer](https://github.com/loren-kimble/photo-library-releases/releases/latest/download/PhotoLibrary-win-Setup.exe)**
(Windows 10 and 11), or see the page about it: https://loren-kimble.github.io/photo-library-releases/

## Installing

1. Open `PhotoLibrary-win-Setup.exe`.
2. If Windows says "Windows protected your PC", choose **More info**, check that the publisher is
   **KimbleLabs LLC**, then **Run anyway**. New programs get this until enough people have installed them.
3. It installs for your Windows account only (no administrator password) and opens in your web browser,
   with a short welcome that helps you choose your photos.

It updates itself. To remove it: Windows Settings > Apps > Photo Library > Uninstall. Your photos, and
the hidden `.photolib` folders that hold what Photo Library learned about them, stay where they are.

## What's here

This repository holds Photo Library's releases (the installer and the files it updates from) and the
two enhancement models it downloads when you first sharpen a photo, converted to ONNX
([models](models)). The app's source is not public.

Problems and ideas: in Photo Library, choose Help, then Feedback.

## Open-source software

Photo Library is built on open-source software, each part under its own licence. The installed app has
them all in its `licenses` folder, with `SOURCES.txt`, which lists the libraries used under the LGPL
(FFmpeg, libheif, libde265, LibRaw), their exact versions and where their source is. KimbleLabs will
send the source of any of those, as built for a release, to anyone who asks within three years of that
release: open an issue here.
