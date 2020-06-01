#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT(program, 1.0, sunggon82.kim@lge.com)
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([-Wall foreign subdir-objects])

# Checks for programs.
AC_PROG_CXX
AM_PROG_AR
LT_INIT([dlopen])

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_CONFIG_FILES([
    Makefile
    minus/Makefile
    plus/Makefile
    program/Makefile
])

AC_ARG_WITH([test], 
    AS_HELP_STRING([--with-test], [building test code])
)

AS_IF([test "x$with_test" = "xyes"],
    AC_CONFIG_FILES([
        test/Makefile
    ])
)
AM_CONDITIONAL([TEST], [test x$with_test = xyes])

AC_OUTPUT

