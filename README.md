# Yggdrasil Networl subnet collision search Proof-of-Concept

Simple modification of SimpleYggGen miner for Proof-of-Concept about its possible to find two keys with same Subnet address.

Application select (filter) only Keys who makes Addresses with same 3 bytes "head", and use Subnet "tail" of 4 bytes to search "collisions" with previously mined Keys. (in Yggdrasil Network (v0.4) first byte of address is always same, so only 7 bytes in IPv6 Subnet is important).

# Requirements

64-bit OS, 4 Gb free memory.

Windows build (via MSYS easy script)

Linux build (make yourself).

# Some statistics

In single test run:

Keys generated: 2.3x 10^10, Filtered: 1.8x 10^5, Collisions found: 5

Keys generated: 3.4x 10^10, Filtered: 2.6x 10^5, Collisions found: 10

Keys generated: 4.2x 10^10, Filtered: 3.2x 10^5, Collisions found: 15

Keys generated: 4.7x 10^10, Filtered: 3.8x 10^5, Collisions found: 20

Keys generated: 5.3x 10^10, Filtered: 4.1x 10^5, Collisions found: 25
