# SysV-MX-Custom-Init-Scripts
Here we are in 2023, and I'm *still* hand writing init scripts just because I dislike systemd so much!  These are for programs that fell over and died under MX21 (a Linux distribution w/SysV init scripts) when they realized PID 1 was a fraud and a hack.

To recitify that issue in the countless packages and upstreams the devs never knew existed (and I only ran upon by sheer luck[?]), I have thrown together a few scripts.  Bones were grabbed from the __init-system_helpers-1.6.0__ Debian package.  Hopefully that will explain the "at least it works" level of code here.

Good / Fast / Correct:  Pick any two!
