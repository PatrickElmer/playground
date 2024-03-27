<img src="img/logo.svg"></img>

Your new, easy, CLI creator for Python.

<a href="https://patrickelmer.github.io/playground/" target="_blank">Start here</a>

``` py title="hello.py"
from magicli import magicli

def hello(name):
    print("hello", name)

if __name__ == "__main__":
    magicli()
```

```bash hl_lines="1"
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
