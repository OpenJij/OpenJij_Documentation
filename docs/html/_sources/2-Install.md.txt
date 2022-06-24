# Install

## pip

```shell
$ pip install openjij
```

For installation with GPU functions, see the topic below.

## pip (without binary)

### CMake setup

OpenJij needs cmake >= 3.17  
If you want to use setup.py instead of PIP, You will need to install CMake>=3.17.  
We are Highly recommended install CMake via PYPI.  
```shell
$ pip install -U cmake
```


### Install

```shell
$ pip install --no-binary=openjij openjij 
```

If a CUDA compiler is found during installation, OpenJij will automatically compile for the GPU.


## from Github

```shell
$ git clone git@github.com:OpenJij/OpenJij.git
$ cd openjij
$ python -m pip install -vvv .
```

## Note

### Windows enviroment
It has been reported that the installation of OpenJij may fail on Windows.
We recommend using Linux through WSL.


### Report an installation problem

Please report the problem to the issue on Github.

[https://github.com/OpenJij/OpenJij/issues](https://github.com/OpenJij/OpenJij/issues)
