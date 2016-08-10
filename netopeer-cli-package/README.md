This folder contains 2 files
- netopeer-cli.cygport
- netopeer-cli-0.8.0-1.src.patch

There might be a file there 
- netopeer-cli-0.8.0.zip

If not then run 
- cygport netopeer-cli.cygport download

There might also be a folder there 
- netopeer-cli-0.8.0-1.x86_64

To clean it away run: 
- cygport netopeer-cli.cygport clean

Then run (to expand the zip and apply the patch)
- cygport netopeer-cli.cygport prep

Then run (run configure and compile - puts files in build)
- cygport netopeer-cli.cygport compile

Then run (to run make install – puts files in inst)
- cygport netopeer-cli.cygport install

Then run (to zip everything up and put it in the dist folder)
- cygport netopeer-cli.cygport package

Copy the contents of the dist folder up to your web server.
- netopeer-cli/netopeer-cli-0.8.0-1.tar.xz
- netopeer-cli/netopeer-cli-0.8.0-1-src.tar.xz
- netopeer-cli/setup.hint
- netopeer-cli-debuginfo/netopeer-cli-debuginfo-0.8.0-1.tar.xz
- netopeer-cli-debuginfo/setup.hint
