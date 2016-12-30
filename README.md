# oslo-config-generator-test

00

    mkvirtualenv oslo-config-generator-test-venv

01

    pip install -Ur requirements.txt

02

http://docs.openstack.org/developer/oslo.config/generator.html

03

    $ oslo-config-generator --namespace myapp
    ----
    WARNING:stevedore.named:Could not load myapp
    [DEFAULT]
    ----

04

    $ python
    ----
    Python 2.7.12+ (default, Sep 17 2016, 12:08:02)
    [GCC 6.2.0 20160914] on linux2
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    >>> from myapp import opts
    >>> opts
    <module 'myapp.opts' from 'myapp/opts.pyc'>
    >>>
    ----
