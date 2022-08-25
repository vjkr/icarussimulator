# icarus Verilog for Windows

There are 2 ways to install.
1. Using MSYS2 installers
2. Binary installers. (These are available from unsecure website)

## 1. Using MSYS2 installers (Didn't work)
  
    Icarus is preferred. install from msys2.org using exe file
    Download the installer: msys2-x86_64-20220603.exe

    https://packages.msys2.org/package/mingw-w64-i686-iverilog?repo=mingw32
    install pacman -S mingw-w64-i686-iverilog

    ###cOULD not comprehend further steps

## 2. Binary installers.(Worked)
    http://bleyer.org/icarus/ download and install iverilog-v12-20220611-x64_setup.exe
        or second executable file
    refer file for compilation and execution 
    C:\iverilog\samples --> Quick_Start.txt
   ![image](https://user-images.githubusercontent.com/16399079/186598131-52e1b4d9-25e5-4d34-b20f-d4943bcd990e.png)
   
# Compilation, Execution and Waveforms
 Compile it:
iverilog -o dsn counter_tb.v counter.v --->  o indicates object, dsn is name of object. after this step dsn file should be generated.
![image](https://user-images.githubusercontent.com/16399079/186628312-c5dd5f41-cf13-47bd-833e-c6a7785bb8bc.png)
Then run it:
vvp dsn ---> execution will show results and vcd file should be generated.
![image](https://user-images.githubusercontent.com/16399079/186628531-5d7ddd39-83f5-4cba-82b8-bac1283bff59.png)
dumpvcd should point filename and dumpvars should point testbench module name
type finish to exit interactive mode
Then look at the test.vcd waveform:
gtkwave test.vcd & --->  gtkwave window should be seen
![image](https://user-images.githubusercontent.com/16399079/186629944-c0c1db9a-c9b2-4737-b5e8-69ec047644a9.png)







