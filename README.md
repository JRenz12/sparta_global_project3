PYTHON PIPELINE PROJECT
==============================

[![TravisCI](https://travis-ci.org/uber/Python-Sample-Application.svg?branch=master)](https://travis-ci.org/uber/Python-Sample-Application)
[![Coverage Status](https://coveralls.io/repos/uber/Python-Sample-Application/badge.png)](https://coveralls.io/r/uber/Python-Sample-Application)

What Is This??
-------------
Uber released an example application that uses their external API. It is built in Python using flask.

This project creates a development, testing and production environments and uses an automated jenkins pipeline to get the code from GitHub and test the code alongside the testing script. On completion a second job will run, that spins up an AMI using packer.

How To Use This
---------------
1. `vagrant up` This command will spin up the virtual machine, using the provisions from the 'python' & 'nginx' cookbooks.
2. `vagrant shh` You will log into the virtual machine securely as the information is encrypted
3. `cd /app` 
4. Run `pip install -r requirements.txt` to install dependencies
5. Run `python app.py`
6. Navigate to `http://pipeline.local` in your browser


Testing
-------
Automated through jenkins.

