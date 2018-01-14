# ida-patch-macos

Patches IDA's Pirated Database Detection upon opening IDA Pro on macOS.
Since I couldn't find any patches for the macOS Platform, I decided to create a simple patch for bypassing the "protection".

# build instructions
```bash
git clone https://github.com/3n16m4/ida-patch-macos.git
cd ida-patch-macos
mkdir build && cd build
cmake .. && make
```

# usage
```bash
./ida-patch-macos <path to ida directory>
```
**INFO:** default path is usually "/Applications/IDA\ Pro\ 7.0/ida.app/Contents/MacOS"

The tool will automatically patch both libraries (libida.dylib, libida64.dylib) and will create backups before patching.

**NOTE:** This tool does ***NOT*** crack IDA!
