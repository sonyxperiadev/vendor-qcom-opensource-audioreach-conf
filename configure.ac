#                                               -*- Autoconf -*-
# configure.ac -- Autoconf script for audioreach-conf
#

# Process this file with autoconf to produce a configure script

# Requires autoconf tool later than 2.61
AC_PREREQ(2.69)
# Initialize the acdbdata package version 1.0.0
AC_INIT([audioreach-conf],1.0.0)
# Does not strictly follow GNU Coding standards
AM_INIT_AUTOMAKE([-Wall -Werror foreign subdir-objects])
# defines some macros variable to be included by source
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])

# Checks for programs.
AC_PROG_CC
AM_PROG_CC_C_O
AC_PROG_CXX
AC_PROG_LIBTOOL
AC_PROG_AWK
AC_PROG_CPP
AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET
PKG_PROG_PKG_CONFIG

AC_ARG_WITH([qcom],
    AS_HELP_STRING([Use qcom based configuration (default is yes)]),
        [with_qcom=$withval],
	    [with_qcom=yes])
	    AM_CONDITIONAL([VENDOR_QCOM], [test "x${with_qcom}" = "xyes"])

AC_CONFIG_FILES([ \
        Makefile \
	qcom/Makefile \
        qcom/kvh2xml.pc
        ])

AC_OUTPUT
