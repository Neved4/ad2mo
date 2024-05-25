# `ad2mo` - Convert date from Gregorian to Mekadimo

Convert Gregorian "A.D." dates to Mekadimo date format.

###### Originally from: [`mekadimo_date.py`]

## Usage

### AWK version

```console
$ echo $(date -u +"%Y-%m-%d") | ./ad2mo.awk
Printuno 64, 0

$ ./ad2mo.awk
Printuno 64, 0

$ ./ad2mo.awk -v iso_fmt=1
0000-01-66
```

### C version

```console
$ make ad2mo && ./ad2mo
Printuno 64, 0
```

[`mekadimo_date.py`]: https://github.com/lajtomekadimon/desktop-distros-config/blob/main/tiling-wm-config/.mekadimo_date.py
