To start creating the pyang package from scratch, make sure you have git, python 3 and python-setuptools installed on Cygwin 

Check out the pyang code in to github by cloning from https://github.com/mbj4668/pyang.git
~/github/pyang

Then do a full install of pyang following the instructions in the README

> python setup.py install

This will create the following folders and files
- /usr/lib/python3.4/site-packages/pyang-1.6-py3.4.egg
- /usr/bin/yang2dsdl
- /usr/bin/yang2html
- /usr/bin/pyang
- /usr/bin/json2xml


Manually create the folder 
> /usr/share/doc/pyang/

and copy the informational files from the source directory in to it

- $ cp ~/github/pyang/CHANGES /usr/share/doc/pyang/ 
- $ cp ~/github/pyang/LICENSE /usr/share/doc/pyang/
- $ cp ~/github/pyang/README /usr/share/doc/pyang/
- $ cp ~/github/pyang/README.md /usr/share/doc/pyang/
- $ cp ~/github/pyang/TODO /usr/share/doc/pyang/


# Packaging
pyang-package

There are 2 main files
- pyang.cygport
- pyang-1.6-1.src.patch

If necessary create the zip file pyang-1.6.zip through 
> cygport pyang.cygport download

Then call the following to apply the patch and create the src folder
> cygport pyang.cygport prep

From this point on it's a manual process – three files need to be created
- pyang/pyang-1.6-1.tar.xz
- pyang/pyang-1.6-1-src.tar.xz
- pyang/setup.hint

Zip up the contents of the Pyang installation in to the main file 
> $ tar -czvf  ~/pyang-package/pyang-1.6-1.x86_64/dist/pyang/pyang-1.6-1.tar.xz \ /usr/lib/python3.4/site-packages/pyang-1.6-py3.4.egg /usr/bin/yang2dsdl \ /usr/bin/yang2html /usr/bin/pyang /usr/bin/json2xml /usr/share/doc/pyang/

Then zip up the source code in to the source file
> $ cd ~/pyang-package/pyang-1.6-1.x86_64/src/pyang-master
> $ tar -czvf ~/pyang-package/pyang-1.6-1.x86_64/dist/pyang/pyang-1.6-1-src.tar.xz *
