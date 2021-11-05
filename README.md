# gccDppConsoleWin
## Overview
gccDppConsoleWin is the program of k-alpha method. This code gets amplifer and time list data from DP5.
Then output data are gotten by sequentialBayes project. 
## Compile
- gcc 4.8.3 32bit
- C++ version 11
- WinAPI
- WinUSB
## 環境変数 
- Path
  - C:\mingw-w64\i686-4.8.3-posix-dwarf-rt_v3-rev2\mingw32\bin\
## 使い方
1. fluxGraphを起動
1. gccDppConsoleWin.exeを起動
1. sequentialBayes.exeを起動
## コンパイル方法
1. 32bit, gcc 4.8.3のgccでC:\mingw-w64\i686-4.8.3-posix-dwarf-rt_v3-rev2
1. vc7_runtimeの中身をここに張り付ける (e.g. msvcr71.dll)
1. makeall.dat
## Download page
- [Cross Platform Software Developer’s Kit (SDK) – updated September 25, 2017](https://www.amptek.com/software/dp5-digital-pulse-processor-software)
  - gccDppConsoleWin – Demonstrates acquisition using LibUsb (WinUSB Backend or LibUsb direct) communications in a MinGW console window.
