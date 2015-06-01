# DejaGnu
**DejaGnu: a framework for testing other programs**

This is an unofficial verbatim redistribution of the binary&source form of the DejaGnu library (a prerequisite for testing programs like GCC), under the terms of GPL 3.0 license.

This redistribution is under the the same GPL 3.0 license.

Please visit the official website for more details: http://www.gnu.org/software/dejagnu

## Usage
The binary/ folder contains both a tar.gz file and a folder, which are equivalent. You can use either one.

## Compilation notes
### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
```bash
wget ftp://ftp.gnu.org/gnu/dejagnu/dejagnu-1.5.3.tar.gz
tar zxvf dejagnu-1.5.3.tar.gz
mkdir build_dejagnu-1.5.3
cd build_dejagnu-1.5.3
../dejagnu-1.5.3/configure --prefix=/home/steven/install/libdejagnu/1.5.3
make
make check
make install
```
Make sure the **CPPFLAGS** and **LDFLAGS** are empty to prevent unwanted inclusion of other directories at compile time.

### Quality verification
See the "QualityVerification.txt" for the output of "make check".