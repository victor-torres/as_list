[![Build
Status](https://travis-ci.org/victor-torres/as_list.png)](https://travis-ci.org/victor-torres/as_list)

# as_list

## Shortcut for

```python
thing_list = "single"

if not isinstance(thing_list, (list, tuple)):
  thing_list = [thing_list]
  
for thing in thing_list:
  do_something(thing)
```

## Becomes

```python
thing_list = "single"
  
for thing in as_list(thing_list):
  do_something(thing)
```

## Install

```shell
$ pip install git+https://github.com/victor-torres/as_list.git
```
