+++
title = 'FFT_feature'
date = 2024-09-13T10:49:18+08:00
draft = true

+++

# FFT feature

## Feature(特性)

支持2/3/5的幂次的FFT点数(包括支持的点数集合定制化)

支持正变换(FFT)和反变换(IFFT)

支持输入和输入信号功率恒定(归一化)

支持高吞吐率(典型值为大约1 sample/clock)

支持电路规格定制化(trade-off between performance/area)

支持RAM架构和Pipeline架构

## Deliverable(交付件)

Verilog/VHDL code or netlist

HDL model and testbench(Parameterization-specific VHDL and Verilog HDL testbench generation)

C/C++ bit accurate model

Matlab bit accurate model (via mex interface)

Python bit accurate model (via CPython interface)

Document (PDF format)

