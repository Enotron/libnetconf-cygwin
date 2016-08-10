This folder contains 2 files
- libnetconf.cygport
- libnetconf-0.10.0-1.src.patch

There might be a file there 
- libnetconf-0.10.0.zip

If not then run 
- cygport libnetconf.cygport download

There might also be a folder there 
- libnetconf-0.10.0-1.x86_64

To clean it away run: 
- cygport libnetconf.cygport clean

Then run (to expand the zip and apply the patch)
- cygport libnetconf.cygport prep

Then run (run configure and compile - puts files in build)
- cygport libnetconf.cygport compile

Then run (to run make install – puts files in inst)
- cygport libnetconf.cygport install

Then run (to zip everything up and put it in the dist folder)
- cygport libnetconf.cygport package

Copy the contents of the dist folder up to your web server.
- libnetconf/libnetconf-0.10.0-1.tar.xz
- libnetconf/libnetconf-0.10.0-1-src.tar.xz
- libnetconf/setup.hint
