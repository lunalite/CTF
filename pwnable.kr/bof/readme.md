```
socat tcp-listen:1234,reuseaddr,fork exec:./bof
```

Simple buffer overflow. Use pattern_create.rb and pattern_offset.rb to find the offset for variable that is being cmp.
