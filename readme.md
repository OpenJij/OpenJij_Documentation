# OpenJij Python documentation

This is the Python documentation repository for OpenJij.

## before install
```
$ git submodule update -i
$ pip install sphinx
$ pip install recommonmark
```
You may need additional Python packages in the course of installation.

## build

```
$ sphinx-apidoc -f -o ./source/apis ./OpenJij/openjij
$ make html
