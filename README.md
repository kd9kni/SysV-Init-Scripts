# SysV-MX-Custom-Init-Scripts
Here we are in 2023, and I'm *still* hand writing init scripts just because I dislike systemd so much!  These are for programs that fell over and died under MX21 (a Linux distribution w/SysV init scripts) when they realized PID 1 was a fraud and a hack.

To recitify that issue in the countless packages and upstreams the devs never knew existed (and I only ran upon by sheer luck[?]), I have thrown together a few scripts.  Bones were grabbed from the __init-system-helpers-1.6.0__ Debian package.  Hopefully that will explain the "at least it works" level of code here.

Good / Fast / Correct:  Pick any two!

My excuse for creating these monstrosties:

* The preinstalled, defaults on MX21 have nice shims and init scripts to hide the fact that they're not on systemd from the services.  That works great until you go outside the reservation.
* Debian's __init-system-system-helpers__ package has all types of nice, hopefully not-riddled-with-non-obvious-errors and show stopping bugs that make up the scaffolding of my own scripts.  That's why there's such a style and process disconnect in different parts of my whole project.
* Sometimes I make changes to the default install environment, like changing the looging location, because the defaults drive me mad and I have my own thoughts on how my system should be organized.
