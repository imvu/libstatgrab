# Makefile for libstatgrab/docs/saidar
# http://www.i-scream.org/libstatgrab/
# $Id: Makefile.am,v 1.3 2008/05/24 22:30:31 ats Exp $

if MANPAGES
if SAIDAR
man_MANS = saidar.1
endif
endif

EXTRA_DIST = $(man_MANS)

.xml.1:
	docbook2man -N --symlinks $<

