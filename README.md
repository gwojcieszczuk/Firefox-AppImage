## Regular and ESR releases of Mozilla Firefox repackaged as AppImage

[Download AppImages](https://webserver.inode.ws/Firefox-AppImage/)

Source: https://ftp.mozilla.org/pub/firefox/releases/

### List of additional libraries, if missing on a system:

* `libgdk-x11-2.0.so.0.2400.32`
* `libgtk-x11-2.0.so.0.2400.32`

Libraries obtained from Ubuntu 20.04 LTS (amd64) installation.

<br>

### Misc

* Firefox versions 91 and below launched with `MOZ_DISABLE_CONTENT_SANDBOX=1` due to `glibc` incompatibility
* `firefox` process created with `MOZ_USE_XINPUT2=1` to enable kinetic scrolling (coasting)
* Appimage creates new firefox profile named `default-appimage`
* It's recommended to leverage AppImage **portable mode** when launching different versions of Firefox


<br>

### Using AppImage portable mode

#### Advantages of portable mode:
* easy to move around your browser with all the settings from one system to another
* you can store all your browser data on portable drive, network drive, etc.

<br>

* Download AppImage file
* Make AppImage file executable
   ```console
	chmod +x Firefox-115.2.1esr-x86_64.AppImage
   ```
* In the same directory as AppImage file, create folder matching AppImage filename + '.home'
   ```console
	mkdir Firefox-115.2.1esr-x86_64.AppImage.home
   ```
* Launch AppImage file

Entire Firefox profile, settings, etc. will be stored within `Firefox-115.2.1esr-x86_64.AppImage.home` directory. When getting newer version of AppImage, just rename `*.home` folder to match new AppImage filename.


