#  Copyright 2014 Darik Horn <dajhorn@vanadac.com>
#
#  This file is part of SoftEther.
#
#  SoftEther is free software: you can redistribute it and/or modify it under
#  the terms of the GNU General Public License as published by the Free
#  Software Foundation, either version 2 of the License, or (at your option)
#  any later version.
#
#  SoftEther is distributed in the hope that it will be useful, but WITHOUT ANY
#  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
#  FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
#  details.
#
#  You should have received a copy of the GNU General Public License along with
#  SoftEther.  If not, see <http://www.gnu.org/licenses/>.


include $(top_srcdir)/autotools/softether.am

# An empty EXEEXT required for overrides with -Wall and -Werror enabled.
AUTOMAKE_OPTIONS = -Wno-override
EXEEXT =

HAMCOREBUILDER = $(top_builddir)/src/hamcorebuilder/hamcorebuilder

noinst_PROGRAMS = hamcore.se2

hamcore.se2$(EXEEXT): $(HAMCOREBUILDER)
	$(HAMCOREBUILDER) $(top_srcdir)/src/bin/hamcore $@

install-exec-local: hamcore.se2$(EXEEXT)
	$(INSTALL_DATA) -D hamcore.se2$(EXEEXT) $(DESTDIR)$(localstatedir)/lib/softether/hamcore.se2
