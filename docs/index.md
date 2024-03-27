<img src="img/logo.svg"></img>

Your new, easy, CLI creator for Python.

<a href="https://patrickelmer.github.io/playground/" target="_blank">Start here</a>

```python
# hello.py
def hello(name):
    print("hello", name)

import magicli
```

```bash
$ python hello.py --help
Usage:
  hello.py arguments [options]

Arguments:
  name

Options:
  -v, --version  Show version information.
  -h, --help     Show this help message.
```

{!README.md!}
