## Basic usage

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

### Simple implementation

``` py title="hello.py"
def hello(name):
    print("hello", name)

import magicli
```

### Advanced implementation

``` py title="hello.py"
from magicli import magicli

def hello(name):
    print("hello", name)

if __name__ == "__main__":
    magicli()
```

## Annotations

```bash hl_lines="1"
$ python square.py --help
Usage:
  square.py [options]

Options:
  -n, --number   Number to square. (default: 1)
  -v, --version  Show version information.
  -h, --help     Show this help message.
```

### Simple implementation

``` py title="square.py"
def square(number: [int, "Number to square.", "n"] = 1):
    return n * n

import magicli
```

### Advanced implementation

``` py title="square.py"
import magicli
from typing import Annotated

def square(
    number: Annotated[int, "Number to square.", "n"] = 1
):
    return n * n

if __name__ == "__main__":
    magicli()
```