# Copyright (c) 2014 Cisco Systems, Inc.

bin_PROGRAMS = ipv4test timestamptest
ipv4test_SOURCES = test_ipv4.c
ipv4test_CPPFLAGS = -I$(top_srcdir)/src
ipv4test_LDADD = $(top_builddir)/src/libfnr.la
ipv4test_DEPENCENCIES = $(ipv4test_LDADD)

timestamptest_SOURCES = test_timestamp.c
timestamptest_CPPFLAGS = -I$(top_srcdir)/src
timestamptest_LDADD = $(top_builddir)/src/libfnr.la
timestamptest_DEPENCENCIES = $(timestamptest_LDADD)

EXTRA_DIST = generate_ipv4.py

if DEBUG
    AM_CFLAGS = -g3 -O0 -DDEBUG
    AM_CXXFLAGS = -g3 -O0 -DDEBUG
else
    AM_CFLAGS = -O2
    AM_CXXFLAGS = -O2
endif
