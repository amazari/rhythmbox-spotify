dnl Process this file with autoconf to produce a configure script.

AC_PREREQ([2.68])
AC_INIT([rhythmbox-spotify],[1.0])
AC_CONFIG_MACRO_DIR([m4])

AC_CONFIG_HEADERS([config.h])

AM_INIT_AUTOMAKE([1.11])

AC_PROG_CC

LT_PREREQ([2.2])
LT_INIT

pkg_modules="glib-2.0 >= 2.24.1
             gobject-2.0 >= 2.24.1
			 rhythmbox
			 gtk+-3.0
			 libsoup-2.4"
             
PKG_CHECK_MODULES(DEPENDENCIES, [$pkg_modules])

AC_SUBST(DEPENDENCIES_CFLAGS)
AC_SUBST(DEPENDENCIES_LIBS)

AC_CONFIG_FILES([
Makefile
src/Makefile
])

AC_OUTPUT

