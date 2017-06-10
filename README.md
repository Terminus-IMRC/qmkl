# QMKL

QMKL is **Math Kernel Library for VideoCore IV QPU**.
QMKL is **compatible with Intel MKL**
except for double precision etc.

_**This repository is suspended currently!**_

This project has temporarily moved to [Idein Inc.](https://github.com/Idein)
and it's under closed development for better functionality and speed.
We are planning to re-open the code. Please wait a few!

We, Idein Inc., did some object recognition demos
using GoogLeNet accelerated by QMKL on
[Raspberry Pi 3](https://twitter.com/9_ties/status/858291781133148160) and
[Raspberry Pi Zero](https://twitter.com/9_ties/status/858300756092375040).


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
