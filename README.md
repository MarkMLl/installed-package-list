# installed-package-list
Simple scripts to monitor installed packages on Debian.

For the last ten years or so, I've been using a script on my Debian installations that logs the list of installed packages into RCS on every reboot.

I've just added a reporting script which generates this sort of output

<pre>
Assume that the starting state has got basic Debian installed, followed by any
GUI required (e.g. KDE and LxQt). No non-free firmware (e.g. for a Broadcom
NIC) has been installed although /etc/apt/sources.list has been updated to
include the contrib and non-free repositories, the senior user has been added
to the sudo group so that remote operation via SSH may be used but there is
no exposure via XDMCP or VNC. MarkMLl

1.1 -> 1.2
elvis-tiny
firmware-bnx2
firmware-linux-nonfree
pidentd
resolvconf
subversion

1.2 -> 1.3
exim4
sudo

1.3 -> 1.4
postgresql

1.4 -> 1.5
qemu

1.5 -> 1.6
bind9
netpipes

1.6 -> 1.7
binutils
hpacucli
...</pre>

...which is sufficiently useful that I thought it worth sharing.
