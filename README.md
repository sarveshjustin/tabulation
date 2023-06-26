# tabulation
```
module ab (a,b,c,d,f);
  input a,b,c,d;
  output f;
assign f = (~b&~d) | (c&d) | (~a&b&d) | (a&c);
endmodule
```
```
g1 0,2,8,10  0,8,2,10    -0-0  ~b ~d

g2 2,3,10,11 2,10,3,11    -01-  ~b c

g3 3,7,11,15  3,11,7,15   --11   cd

g3 10,11,14,15  10,14,11,15  1-1-  ac

```
