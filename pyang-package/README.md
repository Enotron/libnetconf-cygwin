To start creating the pyang package from scratch, make sure you have git, python 3 and python-setuptools installed on Cygwin 

Check out the pyang code in to github by cloning from https://github.com/mbj4668/pyang.git
~/github/pyang

Then do a full install of pyang following the instructions in the README

python setup.py install

This will create the following folders and files
/usr/lib/python3.4/site-packages/pyang-1.6-py3.4.egg
/usr/bin/yang2dsdl
/usr/bin/yang2html
/usr/bin/pyang
/usr/bin/json2xml

Manually create the folder 
/usr/share/doc/pyang/

and copy the informational files from the source directory in to it
$ cp ~/github/pyang/CHANGES /usr/share/doc/pyang/
$ cp ~/github/pyang/LICENSE /usr/share/doc/pyang/
$ cp ~/github/pyang/README /usr/share/doc/pyang/
$ cp ~/github/pyang/README.md /usr/share/doc/pyang/
$ cp ~/github/pyang/TODO /usr/share/doc/pyang/
