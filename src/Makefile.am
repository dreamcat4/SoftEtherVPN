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


# These components are built as libtool convenience libraries.
SUBDIRS = Mayaqua Cedar

# This is a nodist helper.
SUBDIRS += hamcorebuilder

# These are shared components.
SUBDIRS += libsoftether bin/hamcore

# These are the final build products.
SUBDIRS += vpnserver vpnclient vpnbridge vpncmd

# This is a daemon for upstart and systemd.
SUBDIRS += softetherd
