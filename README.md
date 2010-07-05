# jsbtree

A direct brute force port of the Conquex cnxLabs B+ tree Javascript
implementation by Stoyan Pedev to a non-browser NodeJS and GromJS
environment. The original code is @ http://blog.conquex.com/?p=84

License: MIT - http://www.opensource.org/licenses/mit-license.php

Examples on a Core Duo T4400  @ 2.20GHz

### GromJS v1.7.10 (Spidermonkey 1.7.0)

    ~ gromjs jsbtree_test.js
    Populate B+-tree elapsed time: 7.869000196456909
    Populate object elapsed time: 1.9600000381469727
    Populate array elapsed time: 2.1029999256134033
    Search B+-tree elapsed time: 0.0019998550415039062
    Search object elapsed time: 0
    Search array elapsed time: 93.59600019454956
    Range search B+-tree elapsed time: 0
    Range search object elapsed time: 0.26799988746643066
    Range search array elapsed time: 0.35700011253356934

### NodeJS v0.1.100 (V8 ?)...

    ~ node jsbtree_test.js
    Populate B+-tree elapsed time: 0.9129998683929443
    Populate object elapsed time: 1.0780000686645508
    Populate array elapsed time: 0.4939999580383301
    Search B+-tree elapsed time: 0
    Search object elapsed time: 0
    Search array elapsed time: 6.322000026702881
    Range search B+-tree elapsed time: 0
    Range search object elapsed time: 0.315000057220459
    Range search array elapsed time: 0.023999929428100586
