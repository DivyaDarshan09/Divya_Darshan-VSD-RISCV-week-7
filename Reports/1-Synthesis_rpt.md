## Synthesis Report

### VSDbabysoc -  Netlist Statistics

```
=== vsdbabysoc ===
+----------------------------------------------------------------------------------+
|                               Netlist Statistics                                  |
+----------------------------------------------------------------------------------+

Local Count (excluding submodules)
Local Area  (excluding submodules)

   6715    wires  
   6715    wire bits  
   1285    public wires  
   1285    public wire bits  
      7    ports  
      7    port bits  

+----------------------------------------------------------------------------------+
|                                 Standard Cells                                    |
+----------------------------------------------------------------------------------+
|  Count      Total Area     Cell Type                                              |
+----------------------------------------------------------------------------------+

      1            ?         avsddac  
      1            ?         avsdpll  

      1       11.261         sky130_fd_sc_hd__a2111o_1  
      6       52.550         sky130_fd_sc_hd__a2111oi_0  
      8       70.067         sky130_fd_sc_hd__a211o_1  
     26      195.187         sky130_fd_sc_hd__a211oi_1  
     17      127.622         sky130_fd_sc_hd__a21boi_0  
     31      232.723         sky130_fd_sc_hd__a21o_1  
    884     4420.000         sky130_fd_sc_hd__a21oi_1  
      7       61.309         sky130_fd_sc_hd__a21oi_2  
     15      150.144         sky130_fd_sc_hd__a221o_1  
     37      324.061         sky130_fd_sc_hd__a221oi_1  
     24      210.202         sky130_fd_sc_hd__a22o_1  
    222     1670.000         sky130_fd_sc_hd__a22oi_1  
      1       21.270         sky130_fd_sc_hd__a22oi_4  
      1       11.261         sky130_fd_sc_hd__a2bb2o_2  
      4       35.034         sky130_fd_sc_hd__a2bb2oi_1  
      2       20.019         sky130_fd_sc_hd__a311o_1  
     15      131.376         sky130_fd_sc_hd__a311oi_1  
      8       70.067         sky130_fd_sc_hd__a31o_2  
     53      331.568         sky130_fd_sc_hd__a31oi_1  
      1       10.010         sky130_fd_sc_hd__a32o_1  
      3       26.275         sky130_fd_sc_hd__a32oi_1  
      3       26.275         sky130_fd_sc_hd__a41oi_1  

      2       12.512         sky130_fd_sc_hd__and2_0  
     10       62.560         sky130_fd_sc_hd__and2_1  
     14       87.584         sky130_fd_sc_hd__and3_1  

     34      127.622         sky130_fd_sc_hd__buf_1  
      9       45.043         sky130_fd_sc_hd__buf_2  
      1        7.507         sky130_fd_sc_hd__buf_4  
      3       33.782         sky130_fd_sc_hd__buf_6  

    548     2060.000         sky130_fd_sc_hd__clkbuf_1  
      4       15.014         sky130_fd_sc_hd__clkinv_1  
      1        3.754         sky130_fd_sc_hd__conb_1  

   1144    22900.000         sky130_fd_sc_hd__dfxtp_1  

      4       80.077         sky130_fd_sc_hd__fa_1  
    100     1251.200         sky130_fd_sc_hd__ha_1  

    104      390.374         sky130_fd_sc_hd__inv_1  

     56      630.605         sky130_fd_sc_hd__mux2_2  
     92      920.883         sky130_fd_sc_hd__mux2i_1  
      1       22.522         sky130_fd_sc_hd__mux2i_4  
     69     1553.990         sky130_fd_sc_hd__mux4_2  

   1461     5484.010         sky130_fd_sc_hd__nand2_1  
     28      175.168         sky130_fd_sc_hd__nand2b_1  
    213     1070.000         sky130_fd_sc_hd__nand3_1  
     40      300.288         sky130_fd_sc_hd__nand3b_1  
     70      437.920         sky130_fd_sc_hd__nand4_1  
      2       17.517         sky130_fd_sc_hd__nand4b_1  

    284     1070.000         sky130_fd_sc_hd__nor2_1  
     52      325.312         sky130_fd_sc_hd__nor2b_1  
     74      370.355         sky130_fd_sc_hd__nor3_1  
      9       67.565         sky130_fd_sc_hd__nor3b_1  
      1       12.512         sky130_fd_sc_hd__nor3b_2  
     25      156.400         sky130_fd_sc_hd__nor4_1  
      1        8.758         sky130_fd_sc_hd__nor4b_1  

      1       11.261         sky130_fd_sc_hd__o2111a_1  
      8       70.067         sky130_fd_sc_hd__o2111ai_1  
      3       30.029         sky130_fd_sc_hd__o211a_1  
     51      382.867         sky130_fd_sc_hd__o211ai_1  
     30      225.216         sky130_fd_sc_hd__o21a_1  
    397     1990.000         sky130_fd_sc_hd__o21ai_0  
      8       40.038         sky130_fd_sc_hd__o21ai_1  
     10       75.072         sky130_fd_sc_hd__o21bai_1  

     27      236.477         sky130_fd_sc_hd__o221ai_1  
     36      315.302         sky130_fd_sc_hd__o22a_1  
     31      193.936         sky130_fd_sc_hd__o22ai_1  
      2       17.517         sky130_fd_sc_hd__o2bb2ai_1  

      1       10.010         sky130_fd_sc_hd__o311a_1  
      6       52.550         sky130_fd_sc_hd__o311ai_0  
      5       43.792         sky130_fd_sc_hd__o31a_1  
     34      255.245         sky130_fd_sc_hd__o31ai_1  
      1       12.512         sky130_fd_sc_hd__o31ai_2  
      2       20.019         sky130_fd_sc_hd__o32a_1  
      4       35.034         sky130_fd_sc_hd__o32ai_1  

      1       11.261         sky130_fd_sc_hd__o41a_1  
      5       43.792         sky130_fd_sc_hd__o41ai_1  

      
```
---
## Printed Statistics

### Clock Gate

```
=== clk_gate ===

   Number of wires:                  5
   Number of wire bits:              5
   Number of public wires:           5
   Number of public wire bits:       5
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:                  0
```
---
### Rvmyth

```
=== rvmyth ===

   Number of wires:               3948
   Number of wire bits:           6635
   Number of public wires:         269
   Number of public wire bits:    2941
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:               5165
     $ANDNOT                    1412
     $AND                        174
     $DFF_P                      239
     $MUX                        513
     $NAND                        42
     $NOR                         99
     $NOT                         49
     $ORNOT                       74
     $OR                        1322
     $SDFFE_PP0P                 962
     $SDFFE_PP1P                  64
     $SDFF_PP0                     8
     $XNOR                        71
     $XOR                        129
     clk_gate                      7
```
---
### VSDBabySoC

```
=== vsdbabysoc ===

   Number of wires:                  9
   Number of wire bits:             18
   Number of public wires:           9
   Number of public wire bits:      18
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:                  3
     avsddac                         1
     avsdpll                         1
     rvmyth                          1
```
---
## Yosys generic synthesis statistics

- This is Yosys generic synthesis statistics, where the design is still represented using generic gates such as:

- $AND, $OR, $MUX, $DFF_P, $SDFF_PP0, $XOR, $XNOR
- And macros: avsddac, avsdpll
- These are not `physical standard cells yet`.
- They are `technology-independent RTL primitives` generated after initial Yosys synthesis passes.
- So, this block is Technology-independent, generic gate-level netlist.

```
=== design hierarchy ===

   vsdbabysoc                        1
     rvmyth                          1
       clk_gate                      7

   Number of wires:               3992
   Number of wire bits:           6688
   Number of public wires:         313
   Number of public wire bits:    2994
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:               5160
     $ANDNOT                    1412
     $AND                        174
     $DFF_P                      239
     $MUX                        513
     $NAND                        42
     $NOR                         99
     $NOT                         49
     $ORNOT                       74
     $OR                        1322
     $SDFFE_PP0P                 962
     $SDFFE_PP1P                  64
     $SDFF_PP0                     8
     $XNOR                        71
     $XOR                        129
     avsddac                         1
     avsdpll                         1
```
## Technology-mapped netlist

- This is the technology-mapped netlist, after running:
```
dfflibmap
abc -liberty ... # This will automatically run by the script
```
- Now your design is mapped to actual Sky130 standard cells, such as:
```
sky130_fd_sc_hd__nand2_1
sky130_fd_sc_hd__nor2_1
sky130_fd_sc_hd__dfxtp_1 (DFF)
sky130_fd_sc_hd__clkinv_1
```
- Complex gates like sky130_fd_sc_hd__a21oi_1, o21ai_0, etc.
- These are real physical cells available in the Sky130 HD PDK and will be used for placement & routing.
- So this is Technology-mapped standard cell netlist, ready for physical design.

```
Printing statistics.

=== vsdbabysoc ===

   Number of wires:               4737
   Number of wire bits:           6211
   Number of public wires:        4737
   Number of public wire bits:    6211
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:               5913
     avsddac                         1
     avsdpll                         1
     sky130_fd_sc_hd__a2111oi_0      5
     sky130_fd_sc_hd__a211oi_1      10
     sky130_fd_sc_hd__a21boi_0       4
     sky130_fd_sc_hd__a21o_2         3
     sky130_fd_sc_hd__a21oi_1      686
     sky130_fd_sc_hd__a221oi_1     168
     sky130_fd_sc_hd__a22o_2         4
     sky130_fd_sc_hd__a22oi_1      137
     sky130_fd_sc_hd__a311oi_1       4
     sky130_fd_sc_hd__a31o_2         1
     sky130_fd_sc_hd__a31oi_1      315
     sky130_fd_sc_hd__a32oi_1        1
     sky130_fd_sc_hd__a41oi_1       17
     sky130_fd_sc_hd__and2_2        12
     sky130_fd_sc_hd__and3_2         1
     sky130_fd_sc_hd__clkinv_1     568
     sky130_fd_sc_hd__dfxtp_1     1144
     sky130_fd_sc_hd__lpflow_inputiso0p_1      1
     sky130_fd_sc_hd__mux2i_1       14
     sky130_fd_sc_hd__nand2_1      852
     sky130_fd_sc_hd__nand3_1      258
     sky130_fd_sc_hd__nand3b_1       1
     sky130_fd_sc_hd__nand4_1       53
     sky130_fd_sc_hd__nor2_1       428
     sky130_fd_sc_hd__nor3_1        42
     sky130_fd_sc_hd__nor4_1         3
     sky130_fd_sc_hd__o2111ai_1     24
     sky130_fd_sc_hd__o211ai_1      62
     sky130_fd_sc_hd__o21a_1        12
     sky130_fd_sc_hd__o21ai_0      856
     sky130_fd_sc_hd__o21bai_1      12
     sky130_fd_sc_hd__o221a_2        1
     sky130_fd_sc_hd__o221ai_1       3
     sky130_fd_sc_hd__o22a_2         1
     sky130_fd_sc_hd__o22ai_1      135
     sky130_fd_sc_hd__o311ai_0       3
     sky130_fd_sc_hd__o31a_2         1
     sky130_fd_sc_hd__o31ai_1        4
     sky130_fd_sc_hd__o32ai_1        1
     sky130_fd_sc_hd__o41ai_1        2
     sky130_fd_sc_hd__or2_2         12
     sky130_fd_sc_hd__xnor2_1       16
     sky130_fd_sc_hd__xor2_1        34
```