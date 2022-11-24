# notes42

Used for the cours at 42Lausanne

## terminal commands

### cmp

`$ cmp foo bar` compares the two files

`dd if=/dev/urandom of=foo bs=1000 count=1000` writes a 1mb file of random data

### inspecting binary files

[explication video](https://www.youtube.com/watch?v=bWMIpHVRFUo)
[and another to look at later](https://www.youtube.com/watch?v=GV10eIuPs9k)

#### strings

`$ string a.out` to bump all printable string in a.out

#### readelf

`$ readelf  --symbols a.out` list all named symbols used

#### objectdump

`$ objectdump -t ./a.out` simmilar to readelf

`$ objectdump -s ./a.out` see sections

`$ objectdump -d ./a.out` disassemble it

#### strip

`$ strip a.out` removes symbols from binary, makes it a bit smaller and harder to interpret

#### gcc

`-g` flag add debug symbols to binary

### signals

`pgrep a.out` gets the process id for a.out

`kill -INT 543` send a process an interupt signal
`ps -A | less` list process running can also use `ps -e`