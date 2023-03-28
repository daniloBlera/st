# A fork of ST with my configs

Version forked: [0.8.4](https://dl.suckless.org/st/st-0.8.4.tar.gz)

## Patches used

* clipboard     ([st-clipboard-0.8.3.diff][clip])
* iso14755      ([st-iso14755-0.8.3.diff][iso])
* scrollback    ([st-scrollback-0.8.4.diff][scroll])
* xresources    ([st-xresources-20200604-9ba7ecf.diff][xres])
* ligatures     ([st-ligatures-scrollback-0.8.4][ligatures])

[clip]: https://st.suckless.org/patches/clipboard/st-clipboard-0.8.3.diff
[iso]: https://st.suckless.org/patches/iso14755/st-iso14755-0.8.3.diff
[scroll]: https://st.suckless.org/patches/scrollback/st-scrollback-0.8.4.diff
[xres]: https://st.suckless.org/patches/xresources/st-xresources-20200604-9ba7ecf.diff
[ligatures]: https://st.suckless.org/patches/ligatures/0.8.4/st-ligatures-scrollback-20210824-0.8.4.diff

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
