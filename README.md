# `ad2mo` - Convert date from Gregorian to Mekadimo

Convert Gregorian "A.D." dates to Mekadimo date format.

###### Originally from: [`mekadimo_date.py`]

## Usage

### AWK version

Standalone:
```console
$ ./ad2mo.awk
Printuno 64, 0
```

From pipe:
```console
$ echo $(date -u +"%Y-%m-%d") | ./ad2mo.awk
Printuno 64, 0
```

Date in ISO 8601 format:
```console
$ ./ad2mo.awk -v iso_fmt=1
0000-01-64
```

### C version

Compile it with:
```
$ make ad2mo
```

Standalone:
```console
$ ./ad2mo
Printuno 64, 0
```

Piped input:
```console
$ echo $(date -u +"%Y-%m-%d") | ./ad2mo
Printuno 64, 0
```

Date in ISO 8601 format:
```console
$ ./ad2mo -v iso_fmt=1
0000-01-64
```


[`mekadimo_date.py`]: https://github.com/lajtomekadimon/desktop-distros-config/blob/main/tiling-wm-config/.mekadimo_date.py
