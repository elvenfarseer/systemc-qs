---
description: 'bool, sc_bit (deprecated)'
---

# 2-level values with bool



```text
// You shall see warning on sc_bit deprecation
#include "systemc.h"

int sc_main( int argc, char* argv[] ) {
    (void)argc;
    (void)argv;

    sc_bit  sc_enable;
    sc_bit  sc_read_en;
    bool    enable;
    bool    read_en;

    sc_enable = '1';
    cout << "Value of 'sc_enable'  : " << sc_enable << endl;

    sc_read_en = sc_enable;
    cout << "Value of 'sc_read_en' : " << sc_read_en << endl;

    enable = true;
    cout << "Value of 'enable'  : " << enable << endl;

    read_en = enable;
    cout << "Value of 'read_en' : " << read_en << endl;

    sc_enable = '0';
    cout << "Value of 'sc_enable'  : " << sc_enable << endl;

    // bool and sc_bit could be assigned to each other
    read_en = sc_enable;
    cout << "Value of 'read_en' : " << read_en << endl;

    sc_enable = enable;
    cout << "Value of 'sc_enable'  : " << sc_enable << endl;

    return ( 1 );
}
```

