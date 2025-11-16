## Floorplan Final Report in OpenROAD

- After the floorplan stage, OpenROAD generates several timing and power reports. These reports indicate whether the design is physically feasible before moving to placement and routing.

```
==========================================================================
floorplan final report_tns
--------------------------------------------------------------------------
tns max 0.00

==========================================================================
floorplan final report_wns
--------------------------------------------------------------------------
wns max 0.00

==========================================================================
floorplan final report_worst_slack
--------------------------------------------------------------------------
worst slack max 0.27

==========================================================================
floorplan final report_clock_min_period
--------------------------------------------------------------------------
clk period_min = 10.73 fmax = 93.23

==========================================================================
floorplan final report_checks -path_delay min
--------------------------------------------------------------------------
Startpoint: core.CPU_imm_a2[10]$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_imm_a3[10]$DFF_P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: min

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                  0.00    0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock network delay (ideal)
                  0.00    0.00    0.00 ^ core.CPU_imm_a2[10]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     1    0.00    0.03    0.27    0.27 ^ core.CPU_imm_a2[10]$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_imm_a2[10] (net)
                  0.03    0.00    0.27 ^ core.CPU_imm_a3[10]$DFF_P/D (sky130_fd_sc_hd__dfxtp_1)
                                  0.27   data arrival time

                  0.00    0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock network delay (ideal)
                          0.00    0.00   clock reconvergence pessimism
                                  0.00 ^ core.CPU_imm_a3[10]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
                         -0.03   -0.03   library hold time
                                 -0.03   data required time
-----------------------------------------------------------------------------
                                 -0.03   data required time
                                 -0.27   data arrival time
-----------------------------------------------------------------------------
                                  0.31   slack (MET)



==========================================================================
floorplan final report_checks -path_delay max
--------------------------------------------------------------------------
Startpoint: core.CPU_valid_load_a5$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_src1_value_a3[28]$DFF_P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: max

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                  0.00    0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock network delay (ideal)
                  0.00    0.00    0.00 ^ core.CPU_valid_load_a5$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     3    0.01    0.04    0.29    0.29 v core.CPU_valid_load_a5$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_valid_load_a5 (net)
                  0.04    0.00    0.29 v 05430/A (sky130_fd_sc_hd__or4_1)
    44    0.10    0.53    0.98    1.27 v 05430/X (sky130_fd_sc_hd__or4_1)
                                         01114 (net)
                  0.53    0.00    1.27 v 05431/A (sky130_fd_sc_hd__inv_1)
    56    0.15    1.20    1.07    2.34 ^ 05431/Y (sky130_fd_sc_hd__inv_1)
                                         01115 (net)
                  1.20    0.00    2.34 ^ 08797/A2 (sky130_fd_sc_hd__a31oi_1)
     4    0.01    0.25    0.28    2.62 v 08797/Y (sky130_fd_sc_hd__a31oi_1)
                                         03825 (net)
                  0.25    0.00    2.62 v 09692/B1 (sky130_fd_sc_hd__a2111oi_0)
    57    0.15    8.93    6.88    9.50 ^ 09692/Y (sky130_fd_sc_hd__a2111oi_0)
                                         04399 (net)
                  8.93    0.00    9.50 ^ 09939/B1 (sky130_fd_sc_hd__o21ai_0)
     1    0.00    1.03    0.58   10.08 v 09939/Y (sky130_fd_sc_hd__o21ai_0)
                                         04626 (net)
                  1.03    0.00   10.08 v 09953/A2 (sky130_fd_sc_hd__o22a_1)
     1    0.00    0.07    0.52   10.60 v 09953/X (sky130_fd_sc_hd__o22a_1)
                                         core.CPU_src1_value_a2[28] (net)
                  0.07    0.00   10.60 v core.CPU_src1_value_a3[28]$DFF_P/D (sky130_fd_sc_hd__dfxtp_1)
                                 10.60   data arrival time

                  0.00   11.00   11.00   clock clk (rise edge)
                          0.00   11.00   clock network delay (ideal)
                          0.00   11.00   clock reconvergence pessimism
                                 11.00 ^ core.CPU_src1_value_a3[28]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
                         -0.13   10.87   library setup time
                                 10.87   data required time
-----------------------------------------------------------------------------
                                 10.87   data required time
                                -10.60   data arrival time
-----------------------------------------------------------------------------
                                  0.27   slack (MET)



==========================================================================
floorplan final report_checks -unconstrained
--------------------------------------------------------------------------
Startpoint: core.CPU_valid_load_a5$DFF_P
            (rising edge-triggered flip-flop clocked by clk)
Endpoint: core.CPU_src1_value_a3[28]$DFF_P
          (rising edge-triggered flip-flop clocked by clk)
Path Group: clk
Path Type: max

Fanout     Cap    Slew   Delay    Time   Description
-----------------------------------------------------------------------------
                  0.00    0.00    0.00   clock clk (rise edge)
                          0.00    0.00   clock network delay (ideal)
                  0.00    0.00    0.00 ^ core.CPU_valid_load_a5$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
     3    0.01    0.04    0.29    0.29 v core.CPU_valid_load_a5$DFF_P/Q (sky130_fd_sc_hd__dfxtp_1)
                                         core.CPU_valid_load_a5 (net)
                  0.04    0.00    0.29 v 05430/A (sky130_fd_sc_hd__or4_1)
    44    0.10    0.53    0.98    1.27 v 05430/X (sky130_fd_sc_hd__or4_1)
                                         01114 (net)
                  0.53    0.00    1.27 v 05431/A (sky130_fd_sc_hd__inv_1)
    56    0.15    1.20    1.07    2.34 ^ 05431/Y (sky130_fd_sc_hd__inv_1)
                                         01115 (net)
                  1.20    0.00    2.34 ^ 08797/A2 (sky130_fd_sc_hd__a31oi_1)
     4    0.01    0.25    0.28    2.62 v 08797/Y (sky130_fd_sc_hd__a31oi_1)
                                         03825 (net)
                  0.25    0.00    2.62 v 09692/B1 (sky130_fd_sc_hd__a2111oi_0)
    57    0.15    8.93    6.88    9.50 ^ 09692/Y (sky130_fd_sc_hd__a2111oi_0)
                                         04399 (net)
                  8.93    0.00    9.50 ^ 09939/B1 (sky130_fd_sc_hd__o21ai_0)
     1    0.00    1.03    0.58   10.08 v 09939/Y (sky130_fd_sc_hd__o21ai_0)
                                         04626 (net)
                  1.03    0.00   10.08 v 09953/A2 (sky130_fd_sc_hd__o22a_1)
     1    0.00    0.07    0.52   10.60 v 09953/X (sky130_fd_sc_hd__o22a_1)
                                         core.CPU_src1_value_a2[28] (net)
                  0.07    0.00   10.60 v core.CPU_src1_value_a3[28]$DFF_P/D (sky130_fd_sc_hd__dfxtp_1)
                                 10.60   data arrival time

                  0.00   11.00   11.00   clock clk (rise edge)
                          0.00   11.00   clock network delay (ideal)
                          0.00   11.00   clock reconvergence pessimism
                                 11.00 ^ core.CPU_src1_value_a3[28]$DFF_P/CLK (sky130_fd_sc_hd__dfxtp_1)
                         -0.13   10.87   library setup time
                                 10.87   data required time
-----------------------------------------------------------------------------
                                 10.87   data required time
                                -10.60   data arrival time
-----------------------------------------------------------------------------
                                  0.27   slack (MET)



==========================================================================
floorplan final report_power
--------------------------------------------------------------------------
Group                  Internal  Switching    Leakage      Total
                          Power      Power      Power      Power (Watts)
----------------------------------------------------------------
Sequential             4.46e-03   2.48e-04   9.26e-09   4.71e-03  75.7%
Combinational          7.46e-04   7.69e-04   8.60e-09   1.51e-03  24.3%
Clock                  0.00e+00   0.00e+00   0.00e+00   0.00e+00   0.0%
Macro                  0.00e+00   0.00e+00   0.00e+00   0.00e+00   0.0%
Pad                    0.00e+00   0.00e+00   0.00e+00   0.00e+00   0.0%
----------------------------------------------------------------
Total                  5.20e-03   1.02e-03   1.79e-08   6.22e-03 100.0%
                          83.7%      16.3%       0.0%
```
---