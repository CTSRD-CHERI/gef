## Setup

```sh
echo source /path/to/gef.py >> ~/.gdbinit
```

*Note*: The default GDB installation from `pkg64` doesn't support python scripting. We need to build GDB with `--with-python=$(which python3)` when running `./configure`. 

## TODO

- Jemalloc heap manager: identify the heap arenas, visualize heap chunks and bins
- Scan memory for capabilities
