# jsbtree

A direct brute force port of the Conquex cnxLabs B+ tree Javascript
implementation by Stoyan Pedev to a non-browser NodeJS and GromJS
environment. The original code is @ http://blog.conquex.com/?p=84

Examples:

To use with GromJS v1.7.10 (Spidermonkey 1.7.0) comment out...

    //var sys = require('sys');
    function _(msg) {
      print(msg, "\n");
      //sys.puts(msg);
    }

    ~ gromjs jsbtree_test.js
    Populate B+-tree elapsed time: 7.872999906539917
    Populate object elapsed time: 1.940000057220459
    Populate array elapsed time: 2.135999917984009
    Search B+-tree elapsed time: 0.002000093460083008
    Search object elapsed time: 0
    Search array elapsed time: 88.90499997138977
    Range search B+-tree elapsed time: 0
    Range search object elapsed time: 0.2649998664855957
    Range search array elapsed time: 0.3340001106262207

To use with NodeJS v0.1.100 (V8 ?) comment out...

    var sys = require('sys');
    function _(msg) {
      //print(msg, "\n");
      sys.puts(msg);
    }

    ~ node jsbtree_test.js
    Populate B+-tree elapsed time: 0.9009997844696045
    Populate object elapsed time: 1.1070001125335693
    Populate array elapsed time: 0.5039999485015869
    Search B+-tree elapsed time: 0.0010001659393310547
    Search object elapsed time: 0
    Search array elapsed time: 6.431999921798706
    Range search B+-tree elapsed time: 0
    Range search object elapsed time: 0.3529999256134033
    Range search array elapsed time: 0.023000001907348633
