For the original forked project please refer here:
https://github.com/ARM-software/ComputeLibrary

This project was modified thus to be able to be compiled in **Windows 10**.
In order to compile do:

1. Download scons 3.0.1 (or later): https://sourceforge.net/projects/scons/files/scons/
2. Use an appropriate Python packet (I've tested with 2.7.11 and 3.6.4).
3. Install scons to your python (e.g. `/c/scons/python config.py install`)
4. Use Git-Bash for compiling and set the path your cross-compiler tools (e.g. arm-linux-gnueabihf-gcc.exe, etc) as environmental variable. E.g. `export CXX_Path=/e/linaro_6.3.1/bin/`.
5. Call the _scons.py_ from your python packet with your desirable variables: 
   `/c/Programs/Python/Python_3_6/Scripts/scons.py Werror=1 debug=0 neon=1 opencl=0 os=linux arch=armv7a`

