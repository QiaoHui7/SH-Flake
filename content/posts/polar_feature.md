+++
title = 'Polar_feature'
date = 2024-09-13T10:58:10+08:00
draft = true

+++

# Polar CODEC

The product is an efficient Polar encoder/decoder Core solution compliant with 3GPP NR (5G) specifications. The Core is fully validated and has been selected by several early adopters for their 5G SoC. Uplink and Downlink specs are covered.

### Applications:

- 3GPP NR (5G) base station
- 3GPP NR (5G) terminal

### Functional specifications (Downlink):

- CRC handling, with scrambling mask, configurable LFSR init.
- Interleaver for distributed CRC
- Polar encoding/decoding
- Sub-block interleaver
- Bit selection covering shortening, puncturing and repetition

### Functional specifications (Uplink):

- CRC handling
- Parity Check handling
- Polar encoding/decoding
- Sub-block interleaver
- Bit selection covering shortening, puncturing and repetition
- Triangular bit interleaver

### Core features:

- Fully validated Cores (comprehensive factory tests, independant verifications)
- Uplink/Downlink support selectable prior synthesis
- Near optimal error decoding performance with List Successive Cancellation decoder
- Selectable List Size (prior synthesis)
- Dynamic throughput vs error decoding performance trade-off
- Comprehensive monitoring information, incl. metrics for False Alarm Rate improvement
- AXI4-stream interfaces
- Frame-by-frame on-the-fly configuration
- Very high clock frequency achieved on ASIC and FPGA



{{< embed-pdf url="./content/posts/Polar_Example.pdf"  hidePaginator="true" >}}



