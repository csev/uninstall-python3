Uninstall Python3
=================

A simple shell script to un-install Python 3 versions from Mac OS/X.

Of course we all want Python 3 everywhere - but sometimes we want to remove the older version and install
the latest version - or just do a re-install from scratch.   

There is no need to check out this repository - just grab the `uninstall-python3.sh` file and download it
somewhere.

The script is designed to function as a dry run so you can see all that it will do.   To run a dry run, do

    bash uninstall-python3.sh

Examine the output - make sure that it is moving only the expected files.  When you are convinced this will do what you expect, run

    bash uninstall-python3.sh | sudo bash -v

To verify the files are gone, you can re-run

    bash uninstall-python3.sh

It should produce no output.

And then you can happily re-install Python 3!
 
Sample Output (an easy approach)
=============
 
Here is the output of a sample run with the dry run first and the actual run second.  At the very
end, we re-run a dry run to make sure things are gone.
 
    $ bash uninstall-python3.sh
    rm '/usr/local/bin/2to3'
    rm '/usr/local/bin/2to3-3.6'
    rm '/usr/local/bin/easy_install-3.6'
    rm '/usr/local/bin/idle3'
    rm '/usr/local/bin/idle3.6'
    rm '/usr/local/bin/pip3'
    rm '/usr/local/bin/pip3.6'
    rm '/usr/local/bin/pydoc3'
    rm '/usr/local/bin/pydoc3.6'
    rm '/usr/local/bin/python3'
    rm '/usr/local/bin/python3-32'
    rm '/usr/local/bin/python3-config'
    rm '/usr/local/bin/python3.6'
    rm '/usr/local/bin/python3.6-32'
    rm '/usr/local/bin/python3.6-config'
    rm '/usr/local/bin/python3.6m'
    rm '/usr/local/bin/python3.6m-config'
    rm '/usr/local/bin/pyvenv'
    rm '/usr/local/bin/pyvenv-3.6'
    rm -rf '/Library/Frameworks/Python.framework/Versions/3.6'
    rm -rf '/Applications/Python 3.6'
    $ bash uninstall-python3.sh | sudo bash -v
    Password:
    rm '/usr/local/bin/2to3'
    rm '/usr/local/bin/2to3-3.6'
    rm '/usr/local/bin/easy_install-3.6'
    rm '/usr/local/bin/idle3'
    rm '/usr/local/bin/idle3.6'
    rm '/usr/local/bin/pip3'
    rm '/usr/local/bin/pip3.6'
    rm '/usr/local/bin/pydoc3'
    rm '/usr/local/bin/pydoc3.6'
    rm '/usr/local/bin/python3'
    rm '/usr/local/bin/python3-32'
    rm '/usr/local/bin/python3-config'
    rm '/usr/local/bin/python3.6'
    rm '/usr/local/bin/python3.6-32'
    rm '/usr/local/bin/python3.6-config'
    rm '/usr/local/bin/python3.6m'
    rm '/usr/local/bin/python3.6m-config'
    rm '/usr/local/bin/pyvenv'
    rm '/usr/local/bin/pyvenv-3.6'
    rm -rf '/Library/Frameworks/Python.framework/Versions/3.6'
    rm -rf '/Applications/Python 3.6'
    $ bash uninstall-python3.sh
    $

Happy re-installing!
