# QMKL

_**This project is suspended currently!**_

To avoid our competitors use this library illegally,
we, [Idein Inc.](https://github.com/Idein) will develop this library internally.
After we started shipping our products or get off the ground
or in such a situation, we will make our private repository public.
Please wait a few!


QMKL is **Math Kernel Library for VideoCore IV QPU**.
QMKL is **compatible with Intel MKL**
except for double precision etc.


## Requirements

You need to install [qasm2](https://github.com/Terminus-IMRC/qpu-assembler2)
and [qbin2hex](https://github.com/Terminus-IMRC/qpu-bin-to-hex) to compile
this library. Just clone them and do `make && sudo make install`.


## Installation

```
$ git clone https://github.com/Terminus-IMRC/qmkl.git
$ cd qmkl/
$ cmake .
$ make
$ sudo make install
```


## Running tests

```
$ sudo test/sgemm
$ sudo test/scopy
$ sudo test/vsAbs
```

The results are [here](https://gist.github.com/Terminus-IMRC/1ec399a64edcacfc3040baf3c97f0895).
