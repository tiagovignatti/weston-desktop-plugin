AC_PREREQ([2.64])
AC_INIT([desktop plugin],
        [0.1],
        [https://bugs.freedesktop.org],
        [desktop plugin],
        [http://wayland.freedesktop.org/])

AM_INIT_AUTOMAKE([1.11 foreign no-dist-gzip dist-xz])

AM_SILENT_RULES([yes])

# Check for programs
AC_PROG_CC

LT_PREREQ([2.2])
LT_INIT([disable-static])

PKG_PROG_PKG_CONFIG()

PKG_CHECK_MODULES([PLUGIN], [weston >= 1.0.90 pixman-1 xkbcommon])

WAYLAND_SCANNER_RULES(['$(top_srcdir)/protocol'])

AC_CONFIG_FILES([Makefile
		src/Makefile
		protocol/Makefile])

AC_OUTPUT
