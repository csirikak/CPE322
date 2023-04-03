## Lab 1 — GHDL and GTKWave

Windows Binaries of GHDL and GTKWave were downloaded and used for this demonstration.
Please ensure that when running gtkwave to display the output from ghdl, you match the file path of the vcd files accurately.

### Half Adder
```
ghdl -a ha.vhdl
ghdl -a ha_tb.vhdl
ghdl -e ha_tb
ghdl -r ha_tb --vcd=ha.vcd
..\ghdl\ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test
gtkwave ha.vcd
```
![image](https://user-images.githubusercontent.com/32028457/220701204-20725ae3-d01e-4330-9c4a-9d1bd24b5593.png)

### D Flip-Flop
```
ghdl -a dff.vhdl
ghdl -a dff_tb.vhdl
ghdl -e dff_tb
ghdl -r dff_tb --vcd=dff.vcd
gtkwave dff.vcd
```
![image](https://user-images.githubusercontent.com/32028457/220702601-d53f7a85-5192-48da-bbb2-8d7331f6b4f1.png)
