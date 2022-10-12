# C++ Boilerplate
[![Build Status](https://travis-ci.org/dpiet/cpp-boilerplate.svg?branch=master)](https://travis-ci.org/dpiet/cpp-boilerplate)
[![Coverage Status](https://coveralls.io/repos/github/dpiet/cpp-boilerplate/badge.svg?branch=master)](https://coveralls.io/github/dpiet/cpp-boilerplate?branch=master)
---

## Overview

To understand the usage of Valgrind and how its used to make our code robust

- Valgrind
- KCachegrind

## Standard install via command-line
```
git clone --recursive https://github.com/dpiet/cpp-boilerplate
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app
```

## Steps

1. We found two Errors in the whole program, one was present in main.cpp and other in AnalogSignal.cpp.

2. The bug present in main.cpp was corrected by initialising the variable terminal to true.

3. The second bug was present in AnalogSensor.cpp and was corrected by deallocating the memory assigned to the vector pointer.

4. All the valgrind output have been stored in "error_output.txt" and "output_after_fixing_errors.txt" files.

5. The screenshot of KCachegrind is stored as "KCachegrind_output.png" in directory. 