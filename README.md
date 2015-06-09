[![Build
Status](https://travis-ci.org/victor-torres/as_list.png)](https://travis-ci.org/victor-torres/as_list)

# as_list

Verifies it giving object is a list or tuple; if not, returns a list with it as single element.

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
