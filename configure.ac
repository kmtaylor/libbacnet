AC_INIT([libbacnet], [r2858])
AC_CONFIG_AUX_DIR([config])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_HEADERS([config.h])

AM_INIT_AUTOMAKE
AM_SILENT_RULES([yes])

LT_INIT

AC_PROG_CC

AC_ARG_VAR([BAC_SRC], [location of BacNet src files])
AC_ARG_VAR([BAC_PORT], [location of BacNet port files])
AC_ARG_VAR([BAC_OBJECT], [location of BacNet object files])
AC_ARG_VAR([BAC_HANDLER], [location of BacNet handler files])
AC_ARG_VAR([BAC_INCLUDE], [location of BacNet include files])

BAC_SRC="\$(top_srcdir)/../src"
BAC_PORT="\$(top_srcdir)/../ports/linux"
BAC_OBJECT="\$(top_srcdir)/../demo/object"
BAC_HANDLER="\$(top_srcdir)/../demo/handler"
BAC_INCLUDE="\$(top_srcdir)/../include"

AC_ARG_WITH([pkgconfdir],
    AS_HELP_STRING([--with-pkgconfdir=dir],
	[path where pkg-config data will be installed]),
    pkgconfdir="$withval", pkgconfdir="$libdir/pkgconfig")
AC_SUBST(PKGCONF_DIR, "$pkgconfdir")

AC_CONFIG_FILES([
    Makefile
    include/Makefile
    lib/Makefile
    libbacnet.pc
])

AC_OUTPUT
