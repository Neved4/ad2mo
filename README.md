# `ad2mo` - Gregorian to Mekadimo dates! 📟

Convert dates from Gregorian _"A.D."_ to Mekadimo date format.

###### Originally from: [`mekadimo_date.py`]

## Usage

These variants support standalone execution, reading from `stdin` and optionally format the output in [ISO 8601].

### AWK version

Standalone:
```console
$ ./ad2mo.awk
Printuno 64, 0
```

From standard input:
```console
$ echo $(date -u +"%Y-%m-%d") | ./ad2mo.awk
Printuno 64, 0
```

Date in [ISO 8601] format:
```console
$ ./ad2mo.awk -v iso_fmt=1
0000-01-64
```

### C version

Compile with:
```
$ make ad2mo
```

Standalone:
```console
$ ./ad2mo
Printuno 64, 0
```

Standard input:
```console
$ echo $(date -u +"%Y-%m-%d") | ./ad2mo
Printuno 64, 0
```

[ISO 8601] format:
```console
$ ./ad2mo -v iso_fmt=1
0000-01-64
```

## License

This repository is licensed under the terms of the [MIT License].
   
See the [LICENSE](LICENSE) file for details.

[`mekadimo_date.py`]: https://github.com/lajtomekadimon/desktop-distros-config/blob/main/tiling-wm-config/.mekadimo_date.py
[MIT License]: https://opensource.org/license/mit/
[ISO 8601]: https://en.wikipedia.org/wiki/ISO_8601
