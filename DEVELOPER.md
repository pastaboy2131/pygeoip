# Bootstrap manual for developers
_Dependencies: tox, nosetools

### Testing

For testing we are using tox virtualenv-based Python version testing
and nose as test framwork.

Tox will create virtualenvs for all Python version pygeoip supports
and installs the current working tree using the setup.py install script.
Running the tests requires a couple of sample databases found on the
link below.

Maxmind sample databases for testing can be downloaded here:
https://www.defunct.cc/maxmind-geoip-samples.tar.gz (17 MB)

Extract the tarball in the tests directory and run `tox` from the root directory.

This requires a machine with Python 2.6 - 3.6 installed and all dependencies mention in the header.

### TL;DR

There's a Makefile doing all this for you.

    make test
 
 ### Manual testing
 
 In order to perform manual testing do the following below,
 
 Go to the parent directory,
 
 open Terminal or Command Prompt(Windows)
 
 Type  in 
 
 `nosetools /path/file.py`

### Automated testing

In order to the newly perform automated testing,

ensure setup is imported and other dependencies are as well

in your new Python script do the following,

`assert_equals(function)` - sample script will be given in docs directory that tests some of GeoScanner.
