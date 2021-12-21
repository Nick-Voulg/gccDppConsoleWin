# gccDppConsoleWin
## Overview
gccDppConsoleWin is the program of k-alpha method. This code gets amplifer and time list data from DP5.
Then output data are gotten by sequentialBayes project. 
## Send data format
|   DATA[0]   |   DATA[1]   | DATA[2] |   DATA[3]   | DATA[4] | --- |     DATA[2n-1]     |         DATA[2n]          |
|:-----------:|:-----------:|:-------:|:-----------:|:-------:|:---:|:------------------:|:-------------------------:|
|  RECORDS | amplifier[0] | time[0] | amplifier[1] | time[1] | --- |   amplifier[n-1]    |         time[n-1]         |
|      n      |    unsigned long long     |    unsigned long long     |      unsigned long long       |    unsigned long long     | --- | unsigned long long |    unsigned long long     |
- size of data list is unsigned long long
- RECORDS: size of data
- amplifier: channel of detected (0 to 16383)
- time: 16bit + 14bit count (100nS per count)
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