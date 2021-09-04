---
description: Burning time in sc_main
---

# Burning Time

```text
#include "systemc.h"

int sc_main( int argc, char* argv[] ) {
    (void)argc;
    (void)argv;

    cout << "@" << sc_time_stamp() << " Starting simulation" << endl;
    sc_start( 10, SC_US );
    cout << "@" << sc_time_stamp() << " Elapsed time" << endl;
    sc_start( 70, SC_US );
    cout << "@" << sc_time_stamp() << " Elapsed time" << endl;
    cout << "@" << sc_time_stamp() << " Finish Simulation" << endl;

    return ( 0 );
}
```

