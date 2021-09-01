---
description: 'including installation, basic examples and advices for Makefile constructions'
---

# SystemC Tutorial

## Prepare your Rocky Linux Installation for SystemC

Prepare your RockyLinux System for working with SystemC

```bash
sudo dnf install -y epel-release
sudo dnf upgrade -y
sudo dnf group install -y "Development Tools"
```

Check packages

```bash
$ git --version
git version 2.27.0
$ cc --version
cc (GCC) 8.4.1 20200928 (Red Hat 8.4.1-1)
Copyright (C) 2018 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
$ c++ --version
c++ (GCC) 8.4.1 20200928 (Red Hat 8.4.1-1)
Copyright (C) 2018 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

## Getting started with SystemC

Get and isntall SystemC from

```bash
mkdir systemc
cd systemc
wget https://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.3.tar.gz
```

Set up SystemC environment variables

Install according to INSTALL

Add some userful exports to your vimrc to allow for more convinient Makefiles

```bash
export SYSTEMC_HOME=<Prefix>
```



