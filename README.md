Python Grok
========

Introduciton
--------

From original project site  http://code.google.com/p/semicomplete/wiki/Grok

    A powerful pattern-matching/reacting tool
    

Grok is a simplified regular expression parser, using following syntax: 
``` 
	program {
		load-patterns: "patterns/base"
		exec "some program"
	}
	
	match {
		pattern: "IPAddress: %{IP}"
		reaction: "Found: %{IP}" 
	}
```

This will output "Found:" with captured ipaddress behind.

License
--------

*python-grok* source code have been released under the *GPL v3* 
License. Please check the ``LICENSE`` file for more details or visit 
http://www.gnu.org/licenses/gpl-3.0.html


Installing Grok From Source
--------

1. First get grok latest source

    git clone https://github.com/jordansissel/grok
    cd grok
    make create-package
 
or 
    http://code.google.com/p/semicomplete/downloads/detail?name=grok-1.20110708.1.tar.gz


2. Compile and create tar package, then build to rpm
	./rpmbuild -ta grok-xxxxxxxx.tar.gz
	

Get Grok RPM (or other packages will provide later) 
--------

* 

Installing Python Grok
--------

    python setup.py install
    
Use Python Grok
--------

Please read these documents first
* README.md
* docs/html/index.html



Tests
--------
    ./runtests

Misc.
--------