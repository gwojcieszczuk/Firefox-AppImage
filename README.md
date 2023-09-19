## Regular and ESR releases of Mozilla Firefox repacked as AppImage

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
