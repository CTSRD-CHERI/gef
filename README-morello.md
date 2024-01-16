## Setup

```sh
echo source /path/to/gef.py >> ~/.gdbinit
```

*Note*: The default GDB installation from `pkg64` doesn't support python scripting. We need to build GDB with `--with-python=$(which python3)` when running `./configure`. Also, because in a morello box the debug directory is not in `/usr/local64/lib/debug` but in `/usr/lib/debug`, we need to set a custom debug dir with `--with-separate-debug-dir=/usr/lib/debug`.

## Additions

- Fix `vmmap` for FreeBSD and CheriBSD.
- `telescope XXX` shows 0x10-byte aligned addresses.

See also [gef-plugins](https://github.com/CTSRD-CHERI/gef-plugins).
