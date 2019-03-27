SymbiYosys (sby) is a front-end driver program for [Yosys](http://www.clifford.at/yosys)-based formal hardware verification flows. See [http://symbiyosys.readthedocs.io/](http://symbiyosys.readthedocs.io/) for documentation on how to use SymbiYosys.

Many example designs using SymbiYosys have been published on the [ZipCPU blog](http://zipcpu.com).  Please consider browsing the [formal verification page](http://zipcpu.com/formal/formal.html) of the [ZipCPU blog](http://zipcpu.com) for examples and commentary.

## Mini Windows FAQ
* Q: I get `failed to create process` when running `sby.exe`
  
  A: `sby.exe` is a launcher script, and `failed to create process` indicates that launcher couldn't find the Python interpreter.
  Either make sure that the Python interpreter is in the same `bin` directory as the `sby.exe` (set by the `PREFIX` Makefile 
  variable), or try the following invocation:
  
  ```
  make PYTHON=C:\\absolute\\path\\to\\python3.exe PREFIX=/path/to/prefix install
  ```
