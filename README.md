SimpleCoin Multi
================

[![Build Status](https://travis-ci.org/simplecrypto/simplecoin_multi.svg?branch=master)](https://travis-ci.org/simplecrypto/simplecoin_multi)

A multipool version of simplecoin.

Running the dev enviroment
-----------------------------

```` bash
mkvirtualenv scm
pip install -r requirements.txt
pip install -r requirements-dev.txt
pip install -e .
env SIMPLECOIN_CONFIG=example.toml supervisord -c supervisor.conf
```

Running the tests
-----------------------------

```` bash
workon scm
pip install -r requirements-test.txt
nosetests
```

Semi-Functional at the moment!
-----------------------------

**This project is quite green, and does not include some of the code required
to perform automatic exchanging. End-to-end functionality is possible if you
manually exchange the funds (or write your own code). Be prepared to dig into
the code a bit, as a lot of this is pretty green and often poorly documented**

**To get payouts going you'll probably want to look at http://github.com/simplecrypto/simplecoin_rpc_client**
