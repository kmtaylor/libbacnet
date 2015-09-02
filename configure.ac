AC_INIT([libbacnet], [r2858])
AC_CONFIG_AUX_DIR([config])
AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE
AM_SILENT_RULES([yes])

LT_INIT

AC_PROG_LN_S
AC_PROG_CC

AC_ARG_ENABLE([print],
    AS_HELP_STRING([--disable-print], [Disable console printing]),
    AS_IF([test "x$enableval" = "xno"],
	AC_DEFINE([PRINT_ENABLED], 0),	    # --disable-print
	AC_DEFINE([PRINT_ENABLED], 1)),	    # Anything else
    AC_DEFINE([PRINT_ENABLED], 1))	    # Not given

AC_DEFINE([BACAPP_ALL]) # Enable all data types
AC_DEFINE([BACDL_ALL])	# Enable all datalink modes

AC_ARG_ENABLE([file],
    AS_HELP_STRING([--disable-file], [Disable file operations]),
    AS_IF([test "x$enableval" = "xno"],
	[true],				    # --disable-file
	AC_DEFINE([BACFILE])),		    # Anything else
    AC_DEFINE([BACFILE]))		    # Not given

AC_ARG_ENABLE([intrinsic],
    AS_HELP_STRING([--disable-intrinsic], [Disable intrinsic reporting]),
    AS_IF([test "x$enableval" = "xno"],
	[true],				    # --disable-intrinsic
	AC_DEFINE([INTRINSIC_REPORTING])),  # Anything else
    AC_DEFINE([INTRINSIC_REPORTING]))	    # Not given

AC_ARG_ENABLE([bbmd],
    AS_HELP_STRING([--disable-bbmd], [Disable broadcast management device]),
    AS_IF([test "x$enableval" = "xno"],
	AC_DEFINE([BBMD_ENABLED], 0),	    # --disable-bbmd
	AC_DEFINE([BBMD_ENABLED], 1)),	    # Anything else
    AC_DEFINE([BBMD_ENABLED], 1))	    # Not given

AC_ARG_ENABLE([bbmd-client],
    AS_HELP_STRING([--enable-bbmd-client], [Enable BBMD for clients]),
    AS_IF([test "x$enableval" = "xyes"], AC_DEFINE([BBMD_CLIENT_ENABLED])))

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
    patches/Makefile
    libbacnet.pc
])

AC_OUTPUT
