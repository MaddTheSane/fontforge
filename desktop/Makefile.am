# Copyright (C) 2000-2012 by George Williams
# Copyright (C) 2012 by Barry Schwartz
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions are met:
#
# Redistributions of source code must retain the above copyright notice, this
# list of conditions and the following disclaimer.
#
# Redistributions in binary form must reproduce the above copyright notice,
# this list of conditions and the following disclaimer in the documentation
# and/or other materials provided with the distribution.
#
# The name of the author may not be used to endorse or promote products
# derived from this software without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE AUTHOR ``AS IS'' AND ANY EXPRESS OR IMPLIED
# WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
# MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
# EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
# OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
# WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
# OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
# ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

include $(top_srcdir)/mk/layout.am

dist_desktop_DATA = fontforge.desktop
dist_hicolor16x16_DATA = icons/16x16/apps/fontforge.png
dist_hicolor22x22_DATA = icons/22x22/apps/fontforge.png
dist_hicolor24x24_DATA = icons/24x24/apps/fontforge.png
dist_hicolor32x32_DATA = icons/32x32/apps/fontforge.png
dist_hicolor48x48_DATA = icons/48x48/apps/fontforge.png
dist_hicolorscalable_DATA = icons/scalable/apps/fontforge.svg
dist_mimepackages_DATA = fontforge.xml

update-database: update-mime-database update-desktop-database

# The following ignores DESTDIR on purpose. Run after install or
# uninstall.
update-mime-database:
	$(UPDATE_MIME_DATABASE) ${mimedir}

# The following ignores DESTDIR on purpose. Run after install or
# uninstall.
update-desktop-database:
	$(UPDATE_DESKTOP_DATABASE) ${applicationsdir}

EXTRA_DIST = icons/src/icon-16x16-apps-fontforge.svg	\
	icons/src/icon-24x24-apps-fontforge.svg				\
	icons/src/icon-32x32-apps-fontforge.svg

-include $(top_srcdir)/git.mk