# notes42

Used for the cours at 42Lausanne

## terminal commands

### inspecting binary files

[explication video](https://www.youtube.com/watch?v=bWMIpHVRFUo)
[and another to look at later](https://www.youtube.com/watch?v=GV10eIuPs9k)

#### strings

`string a.out` to bump all printable string in a.out

### readelf

`readelf  --symbols a.out` list all named symbols used

#### objectdump

`objectdump -t ./a.out` simmilar to readelf

`objectdump -s ./a.out` see sections

`objectdump -d ./a.out` disassemble it

#### strip

`strip a.out` removes symbols from binary, makes it a bit smaller and harder to interpret

#### gcc

`-g` add debug symbols to binary
