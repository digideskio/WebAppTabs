WebApp Tabs
===========

This is an extension for Thunderbird which allows you to view webapps in
Thunderbird's tabs.

Project Goals
-------------

There are many extensions for viewing webpages in Thunderbird. This isn't what
I think Thunderbird is for, webpages can be viewed in Firefox or whatever
browser you prefer. Thunderbird is my communications centre and I use it to
display communications related webapps like Google+, Google Reader,
Google Groups, etc. and I want to be able to use those easily, opening links in
the default browser where relevant.

The main goals are:

* Allow the user to configure a set of available webapps
* Provide a way for the user to open each webapp in a tab
* Any attempt to open a configured webapp (e.g. from a link in an email or
  anywhere else) should open it in the existing tab for the webapp if one exists
  or a new tab for the webapp in Thunderbird
* Any links clicked in the webapp that are to other sites should open in the
  default browser
* The webapp should behave as well in Thunderbird as it would if opened in
  Firefox

Testing
-------

All fixes should include appropriate automated testing. In order to run the unit
tests the mozbase submodule must first be pulled with `git submodule init` and
`git submodule update`. Then running `python runtests.py` should run the tests
and output any failures.

Building
--------

To build an XPI that can be installed into Thunderbird just run the `build.sh`
command and it will output `webapptabs.xpi` into the current directory. **This
will update any existing file without warning.**

Contributing
------------

As always feel free to fork. This project is MPL/GPL/LGPL tri-licensed. The
issues list contains all the things I know I want to fix, if you have other
ideas then let's talk.
