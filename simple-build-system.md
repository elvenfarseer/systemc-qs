---
description: Describe simple build system based on simplistic Makefile from example
---

# Simple Build System

I advice to start with doing mimic of 3 Makefiles: Makefile for building project, in which you include Makefile.config and Makefile.rules.

This first makefile better to keep withing project folder, other two \(Makefile.config and Makefile.rules\) are shared between projects and shall be kept in some common place. Something like this:

```text
include ../build-unix/Makefile.config

PROJECT := project_name
SRCS    := $(wildcard *.cpp)
OBJS    := $(SRCS:.cpp=.o)

include ../build-unix/Makefile.rules
```

You can and should just change to the `examples` directory within your installation and try to rn every example. This will expose flaws in your flow, like non-valid path to libraries and so on. Fix it and you have your minimal build system.

After that you can easily move to `hello-world` and `burning time` examples, followed by more advanced ones.

