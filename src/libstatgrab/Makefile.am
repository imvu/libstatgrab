# Makefile for libstatgrab/src/libstatgrab
# http://www.i-scream.org/libstatgrab/
# $Id: Makefile.am,v 1.35 2010/02/20 18:17:04 tdb Exp $

if DEPRECATED
include_DEPRECATEDHEADERS = statgrab_deprecated.h
endif
include_HEADERS = statgrab.h $(include_DEPRECATEDHEADERS)
lib_LTLIBRARIES = libstatgrab.la

libstatgrab_la_LDFLAGS = -version-info 8:3:2

if DEPRECATED
libstatgrab_la_DEPRECATEDSOURCES = statgrab_deprecated.c
endif
if MINGW
libstatgrab_la_MINGWSOURCES = win32.c
endif
libstatgrab_la_SOURCES = cpu_stats.c disk_stats.c load_stats.c memory_stats.c network_stats.c os_info.c page_stats.c process_stats.c swap_stats.c user_stats.c tools.c vector.c error.c $(libstatgrab_la_DEPRECATEDSOURCES) $(libstatgrab_la_MINGWSOURCES)

noinst_HEADERS = tools.h vector.h win32.h
