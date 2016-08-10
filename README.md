# libnetconf-cygwin
Patches to compile libnetconf on Cygwin
* pyang does not need to be patched
* libnetconf has a patch file
* netopeer-cli has a patch file
 
The .cygport file of each package points to the location of the source code.

libnetconf depends on the pyang package
netopeer-cli depends on the libnetconf package
