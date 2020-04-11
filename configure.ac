#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([jbigkit], [2.22], [pullmoll@t-online.de])
AM_INIT_AUTOMAKE(subdir-objects)

AC_CONFIG_SRCDIR([libjbig/jbig_ar.c])
AC_CONFIG_MACRO_DIRS([m4])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_MAKE_SET
LT_INIT

# Package check
AC_ARG_ENABLE([tests],
	AS_HELP_STRING([--enable-tests], [Enable codec tests]))

AS_IF([test "x$enable_tests" = "xyes"], [PKG_CHECK_MODULES([CHECK], [check >= 0.9.19])])

# Checks for libraries.
AC_CHECK_LIB([jbig], [jbg_enc_init])
AC_CHECK_LIB([jbig85], [jbg85_enc_init])

# Checks for header files.
AC_CHECK_HEADERS([limits.h stddef.h stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_CHECK_TYPES([ptrdiff_t])

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_CHECK_FUNCS([memchr memset])

AC_CONFIG_FILES([Makefile libjbig/Makefile pbmtools/Makefile test/Makefile
	jbigkit.pc jbigkit85.pc])
AC_OUTPUT
