# uClibc crypt tests
# Licensed under the LGPL v2.1, see the file COPYING.LIB in this tarball.

include ../../.config

ifneq ($(UCLIBC_HAS_CRYPT),y)
TESTS_DISABLED := $(patsubst %.c,%,$(wildcard *.c))
endif

include ../Test.mak

EXTRA_LDFLAGS := -lcrypt

OPTS_crypt = < crypt.input
