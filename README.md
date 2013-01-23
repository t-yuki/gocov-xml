gocov XML (Cobertura) export
============================

__Work in progress. Not useful yet.__

This is a simple helper tool for generating XML output in [Cobertura](http://cobertura.sourceforge.net/) format
for CIs like [Jenkins](https://wiki.jenkins-ci.org/display/JENKINS/Cobertura+Plugin) and others
from [axw/gocov](https://github.com/axw/gocov) output.

Installation
------------

Just type the following to install the program and its dependencies:

    $ go get github.com/axw/gocov/...
    $ go get github.com/AlekSi/gocov-xml

Usage
-----

`gocov-xml` reads from the standard input:

    $ gocov test net/http | gocov-xml > coverage.xml