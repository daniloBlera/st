# A fork of ST (0.8.3) with my configs
## Patches used
*	clipboard	(st-clipboard-0.8.3.diff)
*	scrollback	(st-scrollback-20200419-72e3f6c.diff)
*	xresources	(st-xresources-20190105-3be4cf1.diff)
*	iso14755	(st-iso14755-0.8.3.diff)


st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
