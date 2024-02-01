Galaxy-XSD
==========
[![License](http://img.shields.io/badge/license-MIT-orange.svg?style=flat)](http://opensource.org/licenses/MIT)

**This repository should be considered deprecated, this schema has been updated and migrated into Galaxy [itself](https://github.com/galaxyproject/galaxy/tree/dev/lib/galaxy/tool_util/xsd).**

A Galaxy tool wrapper XML schema definition (XSD).



# History

* The schema has been updated and merged into Galaxy itself (https://github.com/galaxyproject/galaxy/pull/2923)
* Feb-2015 : Pierre Lindenbaum added doc, tests, Java-XML binding file (jxb) for java xml compiler (xjc)  ( https://docs.oracle.com/cd/E19575-01/819-3669/bnbal/index.html )
* 2013 : extraction to standalone and improvements by Jean-Fred
* 2011 : Initial work by John Chilton

# Validating a `tool.xml`

```bash
$ xmllint --noout --schema galaxy.xsd tool.xml 
```

# Creating java code

```bash
$  ${JAVA_HOME}/bin/xjc -b galaxy.jxb galaxy.xsd 
```


# Authors

* Jean-Frédéric @JeanFred
* Pierre Lindenbaum @yokofakun
* John Chilton @jmchilton


# Licence

This code is free software released under the terms of the MIT license.


# See also:

* Galaxy: https://galaxyproject.org/
* Galaxy Tool XML File: https://docs.galaxyproject.org/en/latest/dev/schema.html

