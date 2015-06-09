[![forthebadge](http://forthebadge.com/images/badges/uses-git.svg)](http://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/uses-badges.svg)](http://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/gluten-free.svg)](http://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/makes-people-smile.svg)](http://forthebadge.com)

# as_list [![Build Status](https://travis-ci.org/victor-torres/as_list.png)](https://travis-ci.org/victor-torres/as_list)

Verifies if giving object is list or tuple; if not returns a list with it as single element.

## Why write

```python
thing_list = "single"

if not isinstance(thing_list, (list, tuple)):
  thing_list = [thing_list]
  
for thing in thing_list:
  do_something(thing)
```

## When you can ~lazy~ this

```python
thing_list = "single"
  
for thing in as_list(thing_list):
  do_something(thing)
```

## Install

```shell
$ pip install git+https://github.com/victor-torres/as_list.git
```
