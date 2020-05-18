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
$ git submodule update
$ sphinx-apidoc -f -o ./source/apis ./OpenJij/openjij -d 2
$ make html
```

## Notes

* This Python documentation uses the **Google style** docstrings.
* If the update seems not to be reflected in the HTML files, make sure if the Python files for the documentation are imported from the intended directory when executing `make html`.
