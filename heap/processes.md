---
description: 'Unspawned, spawned. Why, when, how, and differrence'
---

# Processes

From the standard IEEE 1666-2011:

> A _process instance_ is an object of implementation-defined class derived from the class **sc\_object** and created by one of the three macros SC\_METHOD, SC\_THREAD, or SC\_CTHREAD or by calling the function **sc\_spawn**

And this is used in the standard to define a _process:_

> The term _process_ refers to either _process instance_ or to the member function that is associated with a _process instance_ when it is created. The meaning is made clear by the context.

A process could be static or dynamic:

> A _static process_ is a process created during the construction of the module or from the **before\_end\_of\_elaboration** callback.
>
> A _dynamic process_ is a process created from the **end\_of\_elaboration** callback or during the simulation

Seems like _static process_ is something resembling _uvm\_component_ and _dynamic process_ resembling _uvm\_object_ from UVM methodology. But there are more \(maybe unnecessary\) complicated structure in that regard. There are not only _static_ or _dynamic processes_, but also _unspawned_ and _spawned processes_:

> An _unspawned process_ is a process created by invoking one of the three macros SC\_METHOD, SC\_THREAD or SC\_CTHREAD. An _unspawned process_ is typically a static process, but it would be a _dynamic process_ if invoked from the **end\_of\_elaboration** callback
>
> A _spawned process_ is a process created by calling the function **sc\_spawn**. A _spawned process_ is typically a dynamic process, but it would be a _static process_ if **sc\_spawn** is called before the **end\_of\_elaboration**

| Process | Why and how to use |
| :--- | :--- |
| unspawned dynamic |  |
| unspawned static |  |
| spawned dynamic |  |
| spawned static |  |



