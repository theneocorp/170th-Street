# envytools Documentation

envytools is the primary open-source toolkit for reverse engineering NVIDIA GPU hardware and firmware. It includes **envydis** (a disassembler for Falcon microcode and other NVIDIA ISAs), **envyas** (an assembler), and extensive documentation of NVIDIA GPU internals derived from hardware reverse engineering.

This documentation is directly relevant to Falcon security research on the CMP 170HX — envydis is the foundation of the [CAmadeus/falcon-tools](https://github.com/CAmadeus/falcon-tools) toolkit used for disassembling Falcon ucode blobs extracted from VBIOS ROM images, including the DEVINIT scripts and register `0x14118f78` bit-manipulation sequences documented in the [PCIe unlock attempt](runtime-pcie-unlock-attempt.md).

The envytools project documents the Falcon instruction set architecture, memory spaces (IMEM/DMEM), crypto instructions, and the HS/LS/NS privilege model — all essential context for understanding why the CMP 170HX's Ampere-generation Falcon security is difficult to bypass.

{% file src="../.gitbook/assets/envytools-readthedocs-io-en-latest.pdf" %}
