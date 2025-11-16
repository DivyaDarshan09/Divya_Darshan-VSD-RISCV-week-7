## CTS Report

```
==========================================================================
cts final report_tns
--------------------------------------------------------------------------
tns max 0.00

==========================================================================
cts final report_wns
--------------------------------------------------------------------------
wns max 0.00

==========================================================================
cts final report_worst_slack
--------------------------------------------------------------------------
worst slack max 5.93

==========================================================================
cts final report_clock_min_period
--------------------------------------------------------------------------
clk period_min = 5.07 fmax = 197.35

==========================================================================
cts final report_clock_skew
--------------------------------------------------------------------------
Clock clk
   0.77 source latency core.CPU_inc_pc_a2[0]$DFF_P/CLK ^
  -1.01 target latency core.CPU_br_tgt_pc_a3[3]$DFF_P/CLK ^
   0.00 CRPR
--------------
  -0.24 setup skew


==========================================================================
cts final report_checks -path_delay min
--------------------------------------------------------------------------
Startpoint: core.CPU_inc_pc_a2[0]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_inc_pc_a3[0]$DFF_P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: min

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                          0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock source latency
     1    0.21    0.00    0.00    0.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01    0.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.31    0.02    0.33 ^ clkbuf_3_2_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    14    0.34    0.35    0.42    0.75 ^ clkbuf_3_2_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_2__leaf_CLK (net)
                  0.35    0.02    0.77 ^ core.CPU_inc_pc_a2[0]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     2    0.01    0.04    0.40    1.16 v core.CPU_inc_pc_a2[0]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_inc_pc_a2[0] (net)
                  0.04    0.00    1.16 v core.CPU_inc_pc_a3[0]$DFF_P/D (sky130_fd_sc_hd__dfxtp_1)
                                  1.16   data arrival time

                          0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock source latency
     1    0.21    0.00    0.00    0.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01    0.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.31    0.02    0.33 ^ clkbuf_3_2_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    14    0.34    0.35    0.42    0.75 ^ clkbuf_3_2_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_2__leaf_CLK (net)
                  0.35    0.02    0.77 ^ clkbuf_leaf_98_CLK/A (sky130_fd_sc_hd__clkbuf_16)
    15    0.05    0.07    0.24    1.00 ^ clkbuf_leaf_98_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_leaf_98_CLK (net)
                  0.07    0.00    1.00 ^ core.CPU_inc_pc_a3[0]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
                          0.00    1.00   clock reconvergence pessimism
                         -0.05    0.96   library hold time
                                  0.96   data required time
-----------------------------------------------------------------------------
                                  0.96   data required time
                                 -1.16   data arrival time
-----------------------------------------------------------------------------
                                  0.21   slack (MET)



==========================================================================
cts final report_checks -path_delay max
--------------------------------------------------------------------------
Startpoint: core.CPU_src1_value_a3[11]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: max

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                          0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock source latency
     1    0.21    0.00    0.00    0.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01    0.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.32    0.03    0.34 ^ clkbuf_3_6_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    16    0.27    0.28    0.39    0.73 ^ clkbuf_3_6_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_6__leaf_CLK (net)
                  0.28    0.00    0.73 ^ clkbuf_leaf_49_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     7    0.04    0.06    0.22    0.95 ^ clkbuf_leaf_49_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_leaf_49_CLK (net)
                  0.06    0.00    0.95 ^ core.CPU_src1_value_a3[11]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     7    0.06    0.58    0.69    1.64 ^ core.CPU_src1_value_a3[11]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_src1_value_a3[11] (net)
                  0.58    0.00    1.64 ^ 10827/A (sky130_fd_sc_hd__ha_1)
    10    0.03    0.19    0.45    2.09 v 10827/SUM (sky130_fd_sc_hd__ha_1)
                                         00092 (net)
                  0.19    0.00    2.09 v 07812/A (sky130_fd_sc_hd__nor4_1)
     2    0.01    0.38    0.42    2.52 ^ 07812/Y (sky130_fd_sc_hd__nor4_1)
                                         02899 (net)
                  0.38    0.00    2.52 ^ place403/A (sky130_fd_sc_hd__buf_4)
     2    0.01    0.04    0.19    2.71 ^ place403/X (sky130_fd_sc_hd__buf_4)
                                         net402 (net)
                  0.04    0.00    2.71 ^ 07813/B (sky130_fd_sc_hd__nand2_1)
     1    0.01    0.13    0.07    2.78 v 07813/Y (sky130_fd_sc_hd__nand2_1)
                                         02900 (net)
                  0.13    0.00    2.78 v 07814/C1 (sky130_fd_sc_hd__a211oi_1)
     1    0.02    0.64    0.54    3.33 ^ 07814/Y (sky130_fd_sc_hd__a211oi_1)
                                         02901 (net)
                  0.64    0.00    3.33 ^ place387/A (sky130_fd_sc_hd__buf_4)
     2    0.01    0.05    0.23    3.56 ^ place387/X (sky130_fd_sc_hd__buf_4)
                                         net386 (net)
                  0.05    0.00    3.56 ^ 08170/A (sky130_fd_sc_hd__nor2_1)
     1    0.01    0.08    0.05    3.61 v 08170/Y (sky130_fd_sc_hd__nor2_1)
                                         03248 (net)
                  0.08    0.00    3.61 v 08174/A2 (sky130_fd_sc_hd__a21oi_1)
     3    0.03    0.65    0.55    4.16 ^ 08174/Y (sky130_fd_sc_hd__a21oi_1)
                                         03252 (net)
                  0.65    0.00    4.16 ^ 08325/A (sky130_fd_sc_hd__nand2_1)
     2    0.00    0.14    0.13    4.30 v 08325/Y (sky130_fd_sc_hd__nand2_1)
                                         03399 (net)
                  0.14    0.00    4.30 v 08329/B (sky130_fd_sc_hd__and3_1)
     1    0.00    0.04    0.20    4.50 v 08329/X (sky130_fd_sc_hd__and3_1)
                                         03403 (net)
                  0.04    0.00    4.50 v 08333/A3 (sky130_fd_sc_hd__o32ai_1)
     1    0.02    0.55    0.48    4.97 ^ 08333/Y (sky130_fd_sc_hd__o32ai_1)
                                         03407 (net)
                  0.55    0.00    4.97 ^ place349/A (sky130_fd_sc_hd__buf_4)
     3    0.01    0.06    0.23    5.20 ^ place349/X (sky130_fd_sc_hd__buf_4)
                                         net348 (net)
                  0.06    0.00    5.20 ^ 08357/A (sky130_fd_sc_hd__nand2_1)
    12    0.06    0.46    0.31    5.52 v 08357/Y (sky130_fd_sc_hd__nand2_1)
                                         03431 (net)
                  0.46    0.00    5.52 v 09140/A2 (sky130_fd_sc_hd__a311oi_1)
     1    0.00    0.20    0.38    5.90 ^ 09140/Y (sky130_fd_sc_hd__a311oi_1)
                                         00931 (net)
                  0.20    0.00    5.90 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/D (sky130_fd_sc_hd__dfxtp_1)
                                  5.90   data arrival time

                         11.00   11.00   clock clk (rise edge)
                          0.00   11.00   clock source latency
     1    0.21    0.00    0.00   11.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01   11.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30   11.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.31    0.02   11.34 ^ clkbuf_3_0_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    12    0.23    0.24    0.36   11.70 ^ clkbuf_3_0_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_0__leaf_CLK (net)
                  0.24    0.00   11.70 ^ clkbuf_leaf_73_CLK/A (sky130_fd_sc_hd__clkbuf_16)
    13    0.05    0.07    0.22   11.92 ^ clkbuf_leaf_73_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_leaf_73_CLK (net)
                  0.07    0.00   11.92 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/CLK (sky130_fd_sc_hd__dfxtp_1)
                          0.00   11.92   clock reconvergence pessimism
                         -0.09   11.83   library setup time
                                 11.83   data required time
-----------------------------------------------------------------------------
                                 11.83   data required time
                                 -5.90   data arrival time
-----------------------------------------------------------------------------
                                  5.93   slack (MET)



==========================================================================
cts final report_checks -unconstrained
--------------------------------------------------------------------------
Startpoint: core.CPU_src1_value_a3[11]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: max

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                          0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock source latency
     1    0.21    0.00    0.00    0.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01    0.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.32    0.03    0.34 ^ clkbuf_3_6_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    16    0.27    0.28    0.39    0.73 ^ clkbuf_3_6_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_6__leaf_CLK (net)
                  0.28    0.00    0.73 ^ clkbuf_leaf_49_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     7    0.04    0.06    0.22    0.95 ^ clkbuf_leaf_49_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_leaf_49_CLK (net)
                  0.06    0.00    0.95 ^ core.CPU_src1_value_a3[11]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     7    0.06    0.58    0.69    1.64 ^ core.CPU_src1_value_a3[11]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_src1_value_a3[11] (net)
                  0.58    0.00    1.64 ^ 10827/A (sky130_fd_sc_hd__ha_1)
    10    0.03    0.19    0.45    2.09 v 10827/SUM (sky130_fd_sc_hd__ha_1)
                                         00092 (net)
                  0.19    0.00    2.09 v 07812/A (sky130_fd_sc_hd__nor4_1)
     2    0.01    0.38    0.42    2.52 ^ 07812/Y (sky130_fd_sc_hd__nor4_1)
                                         02899 (net)
                  0.38    0.00    2.52 ^ place403/A (sky130_fd_sc_hd__buf_4)
     2    0.01    0.04    0.19    2.71 ^ place403/X (sky130_fd_sc_hd__buf_4)
                                         net402 (net)
                  0.04    0.00    2.71 ^ 07813/B (sky130_fd_sc_hd__nand2_1)
     1    0.01    0.13    0.07    2.78 v 07813/Y (sky130_fd_sc_hd__nand2_1)
                                         02900 (net)
                  0.13    0.00    2.78 v 07814/C1 (sky130_fd_sc_hd__a211oi_1)
     1    0.02    0.64    0.54    3.33 ^ 07814/Y (sky130_fd_sc_hd__a211oi_1)
                                         02901 (net)
                  0.64    0.00    3.33 ^ place387/A (sky130_fd_sc_hd__buf_4)
     2    0.01    0.05    0.23    3.56 ^ place387/X (sky130_fd_sc_hd__buf_4)
                                         net386 (net)
                  0.05    0.00    3.56 ^ 08170/A (sky130_fd_sc_hd__nor2_1)
     1    0.01    0.08    0.05    3.61 v 08170/Y (sky130_fd_sc_hd__nor2_1)
                                         03248 (net)
                  0.08    0.00    3.61 v 08174/A2 (sky130_fd_sc_hd__a21oi_1)
     3    0.03    0.65    0.55    4.16 ^ 08174/Y (sky130_fd_sc_hd__a21oi_1)
                                         03252 (net)
                  0.65    0.00    4.16 ^ 08325/A (sky130_fd_sc_hd__nand2_1)
     2    0.00    0.14    0.13    4.30 v 08325/Y (sky130_fd_sc_hd__nand2_1)
                                         03399 (net)
                  0.14    0.00    4.30 v 08329/B (sky130_fd_sc_hd__and3_1)
     1    0.00    0.04    0.20    4.50 v 08329/X (sky130_fd_sc_hd__and3_1)
                                         03403 (net)
                  0.04    0.00    4.50 v 08333/A3 (sky130_fd_sc_hd__o32ai_1)
     1    0.02    0.55    0.48    4.97 ^ 08333/Y (sky130_fd_sc_hd__o32ai_1)
                                         03407 (net)
                  0.55    0.00    4.97 ^ place349/A (sky130_fd_sc_hd__buf_4)
     3    0.01    0.06    0.23    5.20 ^ place349/X (sky130_fd_sc_hd__buf_4)
                                         net348 (net)
                  0.06    0.00    5.20 ^ 08357/A (sky130_fd_sc_hd__nand2_1)
    12    0.06    0.46    0.31    5.52 v 08357/Y (sky130_fd_sc_hd__nand2_1)
                                         03431 (net)
                  0.46    0.00    5.52 v 09140/A2 (sky130_fd_sc_hd__a311oi_1)
     1    0.00    0.20    0.38    5.90 ^ 09140/Y (sky130_fd_sc_hd__a311oi_1)
                                         00931 (net)
                  0.20    0.00    5.90 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/D (sky130_fd_sc_hd__dfxtp_1)
                                  5.90   data arrival time

                         11.00   11.00   clock clk (rise edge)
                          0.00   11.00   clock source latency
     1    0.21    0.00    0.00   11.00 ^ pll/CLK (avsdpll)
                                         CLK (net)
                  0.02    0.01   11.01 ^ clkbuf_0_CLK/A (sky130_fd_sc_hd__clkbuf_16)
     8    0.30    0.31    0.30   11.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_0_CLK (net)
                  0.31    0.02   11.34 ^ clkbuf_3_0_f_CLK/A (sky130_fd_sc_hd_clkbuf_16)
    12    0.23    0.24    0.36   11.70 ^ clkbuf_3_0_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
                                         clknet_3_0__leaf_CLK (net)
                  0.24    0.00   11.70 ^ clkbuf_leaf_73_CLK/A (sky130_fd_sc_hd__clkbuf_16)
    13    0.05    0.07    0.22   11.92 ^ clkbuf_leaf_73_CLK/X (sky130_fd_sc_hd__clkbuf_16)
                                         clknet_leaf_73_CLK (net)
                  0.07    0.00   11.92 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/CLK (sky130_fd_sc_hd__dfxtp_1)
                          0.00   11.92   clock reconvergence pessimism
                         -0.09   11.83   library setup time
                                 11.83   data required time
-----------------------------------------------------------------------------
                                 11.83   data required time
                                 -5.90   data arrival time
-----------------------------------------------------------------------------
                                  5.93   slack (MET)



==========================================================================
cts final report_check_types -max_slew -max_cap -max_fanout -violators
--------------------------------------------------------------------------

==========================================================================
cts final max_slew_check_slack
--------------------------------------------------------------------------
0.2218235731124878

==========================================================================
cts final max_slew_check_limit
--------------------------------------------------------------------------
1.4862940311431885

==========================================================================
cts final max_slew_check_slack_limit
--------------------------------------------------------------------------
0.1492

==========================================================================
cts final max_fanout_check_slack
--------------------------------------------------------------------------
1.0000000150474662e+30

==========================================================================
cts final max_fanout_check_limit
--------------------------------------------------------------------------
1.0000000150474662e+30

==========================================================================
cts final max_capacitance_check_slack
--------------------------------------------------------------------------
0.005018971860408783

==========================================================================
cts final max_capacitance_check_limit
--------------------------------------------------------------------------
0.03663099929690361

==========================================================================
cts final max_capacitance_check_slack_limit
--------------------------------------------------------------------------
0.1370

==========================================================================
cts final max_slew_violation_count
--------------------------------------------------------------------------
max slew violation count 0

==========================================================================
cts final max_fanout_violation_count
--------------------------------------------------------------------------
max fanout violation count 0

==========================================================================
cts final max_cap_violation_count
--------------------------------------------------------------------------
max cap violation count 0

==========================================================================
cts final setup_violation_count
--------------------------------------------------------------------------
setup violation count 0

==========================================================================
cts final hold_violation_count
--------------------------------------------------------------------------
hold violation count 0

==========================================================================
cts final report_checks -path_delay max reg to reg
--------------------------------------------------------------------------
Startpoint: core.CPU_src1_value_a3[11]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: max

  Delay    Time   Description
---------------------------------------------------------
   0.00    0.00   clock clk (rise edge)
   0.00    0.00   clock source latency
   0.00    0.00 ^ pll/CLK (avsdpll)
   0.31    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.41    0.73 ^ clkbuf_3_6_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
   0.22    0.95 ^ clkbuf_leaf_49_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.00    0.95 ^ core.CPU_src1_value_a3[11]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
   0.69    1.64 ^ core.CPU_src1_value_a3[11]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
   0.45    2.09 v 10827/SUM (sky130_fd_sc_hd__ha_1)
   0.42    2.52 ^ 07812/Y (sky130_fd_sc_hd__nor4_1)
   0.19    2.71 ^ place403/X (sky130_fd_sc_hd__buf_4)
   0.07    2.78 v 07813/Y (sky130_fd_sc_hd__nand2_1)
   0.54    3.33 ^ 07814/Y (sky130_fd_sc_hd__a211oi_1)
   0.23    3.56 ^ place387/X (sky130_fd_sc_hd__buf_4)
   0.05    3.61 v 08170/Y (sky130_fd_sc_hd__nor2_1)
   0.55    4.16 ^ 08174/Y (sky130_fd_sc_hd__a21oi_1)
   0.14    4.30 v 08325/Y (sky130_fd_sc_hd__nand2_1)
   0.20    4.50 v 08329/X (sky130_fd_sc_hd__and3_1)
   0.48    4.97 ^ 08333/Y (sky130_fd_sc_hd__o32ai_1)
   0.23    5.20 ^ place349/X (sky130_fd_sc_hd__buf_4)
   0.31    5.52 v 08357/Y (sky130_fd_sc_hd__nand2_1)
   0.38    5.90 ^ 09140/Y (sky130_fd_sc_hd__a311oi_1)
   0.00    5.90 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/D (sky130_fd_sc_hd__dfxtp_1)
           5.90   data arrival time

  11.00   11.00   clock clk (rise edge)
   0.00   11.00   clock source latency
   0.00   11.00 ^ pll/CLK (avsdpll)
   0.31   11.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.38   11.70 ^ clkbuf_3_0_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
   0.22   11.92 ^ clkbuf_leaf_73_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.00   11.92 ^ core.CPU_Xreg_value_a4[26][27]$SDFFE_PP0P/CLK (sky130_fd_sc_hd__dfxtp_1)
   0.00   11.92   clock reconvergence pessimism
  -0.09   11.83   library setup time
          11.83   data required time
---------------------------------------------------------
          11.83   data required time
          -5.90   data arrival time
---------------------------------------------------------
           5.93   slack (MET)



==========================================================================
cts final report_checks -path_delay min reg to reg
--------------------------------------------------------------------------
Startpoint: core.CPU_inc_pc_a2[0]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_inc_pc_a3[0]$DFF_P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: min

  Delay    Time   Description
---------------------------------------------------------
   0.00    0.00   clock clk (rise edge)
   0.00    0.00   clock source latency
   0.00    0.00 ^ pll/CLK (avsdpll)
   0.31    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.43    0.75 ^ clkbuf_3_2_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
   0.02    0.77 ^ core.CPU_inc_pc_a2[0]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
   0.40    1.16 v core.CPU_inc_pc_a2[0]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
   0.00    1.16 v core.CPU_inc_pc_a3[0]$DFF_P/D (sky130_fd_sc_hd__dfxtp_1)
           1.16   data arrival time

   0.00    0.00   clock clk (rise edge)
   0.00    0.00   clock source latency
   0.00    0.00 ^ pll/CLK (avsdpll)
   0.31    0.31 ^ clkbuf_0_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.43    0.75 ^ clkbuf_3_2_f_CLK/X (sky130_fd_sc_hd_clkbuf_16)
   0.26    1.00 ^ clkbuf_leaf_98_CLK/X (sky130_fd_sc_hd__clkbuf_16)
   0.00    1.00 ^ core.CPU_inc_pc_a3[0]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
   0.00    1.00   clock reconvergence pessimism
  -0.05    0.96   library hold time
           0.96   data required time
---------------------------------------------------------
           0.96   data required time
          -1.16   data arrival time
---------------------------------------------------------
           0.21   slack (MET)



==========================================================================
cts final critical path target clock latency max path
--------------------------------------------------------------------------
0

==========================================================================
cts final critical path target clock latency min path
--------------------------------------------------------------------------
0

==========================================================================
cts final critical path source clock latency min path
--------------------------------------------------------------------------
0

==========================================================================
cts final critical path delay
--------------------------------------------------------------------------
5.8983

==========================================================================
cts final critical path slack
--------------------------------------------------------------------------
5.9328

==========================================================================
cts final slack div critical path delay
--------------------------------------------------------------------------
100.584914

==========================================================================
cts final report_power
--------------------------------------------------------------------------
Group                  Internal  Switching    Leakage      Total
                          Power      Power      Power      Power (Watts)
----------------------------------------------------------------
Sequential             4.36e-03   4.17e-04   9.27e-09   4.78e-03  38.9%
Combinational          8.62e-04   2.14e-03   9.86e-09   3.00e-03  24.4%
Clock                  2.35e-03   2.15e-03   1.95e-09   4.50e-03  36.7%
Macro                  0.00e+00   0.00e+00   0.00e+00   0.00e+00   0.0%
Pad                    0.00e+00   0.00e+00   0.00e+00   0.00e+00   0.0%
----------------------------------------------------------------
Total                  7.57e-03   4.71e-03   2.11e-08   1.23e-02 100.0%
                          61.7%      38.3%       0.0%
```