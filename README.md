## MinTeXt

- A file format that crams characters into less than 1 byte
- Not meant to be perfect!

## Supported chars (63)
`abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789 ` (including space)

## Docs
```c
uint8_t * str_mt(const char * data); // takes string, converts to byte array
char * mt_str(uint8_t * data); // takes byte array, converts to string
```
> nuff said
## Examples
### Storing the word `lizard`
```
-rw-r--r-- 1 werdl werdl     5 Dec 12 19:30 lizard.mtx
-rw-r--r-- 1 werdl werdl     6 Dec 11 19:26 lizard.txt
```

### Storing something longer
`Fourty Two is The Answer To Life The Universe And Everything`
- Best done with the C API
- Still works with files, just the odd bizarre char (don't know why, C API works)
