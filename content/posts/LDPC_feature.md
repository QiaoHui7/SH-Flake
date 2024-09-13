+++
title = 'LDPC_feature'
date = 2024-09-13T10:44:24+08:00
draft = true

+++





# LDPC Feature

## Feature(特性)

AXI-stream interface(refer to AXI spec)

支持单独译码器(decoder only)

支持单独编码器(encoder only)

LLR位宽可以灵活配置

(可选)支持基于NR标准的速率匹配 TX (NR rate-matching)

(可选)支持基于NR标准的解速率匹配 RX (NR de-rate-matching)

(可选)支持基于NR标准的HARQ合并 (NR HARQ combine)

(可选)NR LDPC CBGTI (refer to spec)

## Deliverable(交付件)

Verilog/VHDL code or netlist

HDL model and testbench

C/C++ bit accurate model

Matlab bit accurate model (via mex interface)

Python bit accurate model (via CPython interface)

Document (PDF format)

## Reference

Creonic LDPC full decoder chain 在Xilinx中的资源消耗对照

Xilinx 7z045 / 112,731 LUTs / 103,946 FFs / BRAMs(18k/36k) (13/351) / DSP48E 0 / Freq 150MHz
(Xilinx 7z020是Xilinx 7z045的大约1/4)

LDPC decoder Throughput: 574M bit/s

performance:

BLER 1e-4 for BG-1 Es/N0 =  6.24dB (QPSK, k = 8448, R = 22/27)
BLER 1e-4 for BG-1 Es/N0 = -0.34dB (QPSK, k = 8448, R = 22/68)

BLER 1e-4 for BG-2 Es/N0 =  3.49dB (QPSK, k = 3840, R = 10/17)
BLER 1e-4 for BG-2 Es/N0 = -3.00dB (QPSK, k = 3840, R = 10/52)

default bit width 6-bits

### Functional specifications (encoder):

- CRC encoding
- Filler bits insertion/removal
- LDPC encoding (basegraph1 and 2, all Z-values)
- Rate matching (incl. repetition)
- Bit-level interleaver
- Support of WiFi (optional)
- Transport Block level processing (optional)

### Functional specifications (decoder):

- Bit-level de-interleaver
- HARQ combining
- Inverse Rate matching (incl. repetition)
- Filler bits insertion/removal
- LDPC decoding (basegraph1 and 2, all Z-values)
- CRC decoding
- Soft-output interface (optional)
- Support of WiFi (optional)
- Reencoded output stream (optional)
- Transport Block level processing (optional)

### Core features:

- Fully validated Cores (comprehensive factory tests, independant verifications)
- Advanced HARQ combining / stream compression
- Versatile Decoding algorithm profiles
- Scalable throughput design
- Very high clock frequency achieved on ASIC process
- Multi-Gigabit range throughput
- Scalable design (three throughput profiles)
- AXI4-stream interfaces
- Frame-by-frame on-the-fly configuration
- Comprehensive monitoring information (syndrome check, SNR indicator,...)
- Efficient iteration-stopping feature

