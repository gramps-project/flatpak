# Gramps Flatpak
These are the manifest and data files required to make a Gramps Flatpak

The flatpak is available on flathub at https://flathub.org/apps/details/org.gramps_project.Gramps
The Gramps flatpak contains dependencies and works with flathub runtimes to work independently regardless of the linux distribution.  There are also dependencies for some third party add-ons like Graphview and Network Chart.

# List of Included Dependencies
Dependencies confirmed in the Gnome flatpak platform (Gnome 50 as of Gramps 6.1.0-beta1--1 flatpak):
- python3
- gtk
- pygobject
- cairo
- pango
- pangocairo
- librsvg2

Dependencies added to the flatpak
- orjson
- osmgpsmap with its libsoup dependency
- graphviz and pygraphviz
- PyICU
- ghostscript
- gspell
- pillow
- exiv2 and gexiv2
- geocodeglib
- goocanvas
- networkx
- python-imagesize
- TTF-Freefonts
- python-fontconfig
- pycountry
- requests with its charset_normalizer, urllib3, and idna dependencies
- certifi

To request another prerequisite be added to support another Gramps add-on, you can request it at the gramps project flatpak github.

https://github.com/gramps-project/flatpak

https://github.com/flathub/org.gramps_project.Gramps

Also, the old version of Berkeley Database (BSDDB3) that was included with the Gramps 5.0 and 5.1 flatpaks was dropped starting with Gramps 5.2. An old archived flatpak with BSDDB3 is available at the gramps-project github https://github.com/gramps-project/flatpak/releases/tag/v5.1.6-1 to facilitate the conversion of old Gramps databases from BSDDB3 to the current SQLite.

In 2021, Gnu RCS 5.10.0 could be compiled into the flatpak. The newer tar.lz archives and some formatting issues now make RCS fail to compile.  If anyone can get it to compile into the Gramps flatpak, you are welcome to submit a PR to https://github.com/gramps-project/flatpak

Please make regular full backups of your important genealogy files, and include any attached media files for your genealogy in your backups for your convenience.
