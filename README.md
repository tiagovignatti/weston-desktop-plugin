# Desktop Shell plugin

This repository just holds a standalone copy of the Shell Desktop plugin from
Weston freedesktop.org -- simple, easy to understand and modularized here.

Relies on Weston and its SDK for spawning the plugin process with the right
API. It is using wl_shell_surface high-level wrapper of wl_surface for
defining the desktop UI aspects and semantics, as defined in Wayland core
protocol.

## More

http://vignatti.wordpress.com/2013/03/05/ui-customization-on-wayland/
