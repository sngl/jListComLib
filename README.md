# README

Java library for Mac and Windows that allows to list all the Arduino connected to the computer.
Complete sources in:

src_mac/ for the Mac version.
src_win/ for the Windows version


Test program and library binary in test/

### Note:

To compile under Windows [MinGW](http://www.mingw.org/) and jdk are required 

command line: g++ -Wall -D_JNI_IMPLEMENTATION_ -Wl,--kill-at  -I"C:\Program Files (x86)\Java\jdk1.7.0_40\include" -I"C:\Program Files (x86)\Java\jdk1.7.0_40\include\win32" -shared listCom_java.cpp -o bin\listCom.dll -lsetupapi -DWIN


To compile under OSX:  g++ -Wall -D_JNI_IMPLEMENTATION_ -shared listCom.cpp -o bin/liblistCom.dylib -lutil -framework CoreFoundation -framework IOKit -DMAC

