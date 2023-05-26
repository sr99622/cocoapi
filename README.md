
# pycocotools

This is a fork of the original [cocoapi](https://github.com/cocodataset/cocoapi), with bug fixes and packaging improvements.

This is also the source of the pypi package `pycocotools`, available for download at [pypi](https://pypi.org/project/pycocotools/).

Changes in this fork include:
* Add CircleCI tests
* Support pip-installation correctly
* Support windows
* Don't import matplotlib unless needed
* Close file handle after openning
* Fix a small bug in rleToBbox
* Fix a segfault in RLE decoding
* Fix deprecated usage of other libraries

For compatibility, we will not make any API changes or non-bug behavior changes to the existing APIs of the official cocoapi.

## Instructions for maintainers: to build a sdist package:
```
python -m build --sdist ./PythonAPI
```

## to build a wheel
```
python -m build --wheel ./PythonAPI
```
