---
description: Hello world in SystemC
---

# Hello World

```cpp
#include "systemc.h"

SC_MODULE ( hello_world ) {

    SC_CTOR ( hello_world ) {
        // Nothing in constructor
    }

    void say_hello() {
        cout << "Hello World!" << endl;
    }

};

int sc_main( int argc, char* argv[] ) {
    (void)argc;
    (void)argv;
    hello_world hello( "HELLO" );
    hello.say_hello();
    return ( 0 );
}

```

