# OpenJij Python documentation

This is the Python documentation repository for OpenJij.

## before install

You need Pipenv to build this document

```
$ git submodule update -i
$ pipenv install
$ pipenv shell
```

## build document

```
$ git submodule update
$ cd Openjij
$ pipenv run python setup.py install
$ cd ..
$ pipenv run sphinx-apidoc -f -o ./source/apis ./OpenJij/openjij -d 2
$ pipenv run make html
```

## Notes

* This Python documentation uses the **Google style** docstrings.
* If the update seems not to be reflected in the HTML files, make sure if the Python files for the documentation are imported from the intended directory when executing `make html`.
* **Feel free to throw issues if you find typo in the documents!**
