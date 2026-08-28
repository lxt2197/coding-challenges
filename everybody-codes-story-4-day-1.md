**EVERYBODY CODES**  
**Story 4 - Day 1**

Part 1
```
=LET(inp, A1:A10,
     end, LAMBDA(seq,
                 TAKE(REDUCE(0,--TEXTSPLIT(seq,","),
                             LAMBDA(pth,stp,
                                    LET(prv,TAKE(pth,-1),
                                        VSTACK(pth,
                                               IF(OR(prv-stp<0,ISNUMBER(XMATCH(prv-stp,pth))),
                                                  prv+stp,
                                                  prv-stp))))),
                 -1)),
     SUM(MAP(inp,end)))
```

Part 2
```

```

Part 3
```

```
