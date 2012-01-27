special_shells
==============

These are home-grown scripts which are used as users' shells for various
purposes

accept_AUP
----------

This is the shell a user initially gets when they first activate their account. 
They keep this shell until they accept the AUP, so that by definition anyone
with a proper shell on a netsoc machine has accepted the AUP.

If the user accepts the AUP, they are prompted to bind to LDAP (via
[nd](http://github.com/netsoc/nd/)), and their shell is set to the default
shell (currently set in LDAP as /bin/bash).

bold, expired, renew and dead
-----------------------------

These older scripts used to be used on spoon and matrix to prevent bold, expired
non-renewed and dead accounts from logging in. These days they've been replaced
by groups in LDAP, and a Match Group clause in /etc/sshd_config.
