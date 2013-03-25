moduledir = @libdir@/weston
module_LTLIBRARIES = desktop-shell.la

AM_CPPFLAGS =                                   \
        -DMODULEDIR='"$(moduledir)"'            \
        -DLIBEXECDIR='"$(libexecdir)"'

desktop_shell = desktop-shell.la
desktop_shell_la_LDFLAGS = -module -avoid-version
desktop_shell_la_LIBADD = $(PLUGIN_LIBS)
desktop_shell_la_CFLAGS = $(GCC_CFLAGS) $(PLUGIN_CFLAGS)
desktop_shell_la_SOURCES =                      \
	shell.c                                 \
	desktop-shell-protocol.c                \
	desktop-shell-server-protocol.h		\
	config-parser.c				\
	config-parser.h

BUILT_SOURCES =                                 \
	desktop-shell-protocol.c                \
	desktop-shell-server-protocol.h         \
	input-method-protocol.c                 \
	input-method-server-protocol.h          \
	workspaces-server-protocol.h		\
	workspaces-protocol.c

CLEANFILES = $(BUILT_SOURCES)

@wayland_scanner_rules@
