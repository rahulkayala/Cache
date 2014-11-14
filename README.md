Cache
=====

This is a L1 Cache simulator which a capacity of 2^C  bytes with a Block size of 2^B bytes per block and with associativity S.
The simulator also models a strided prefetcher which prefetches K blocks on 2 consecutive misses.
It has a Victim Cache of V blocks.
The simulator accepts a trace file modelled along the lines of a SPEC Benchmark where each line is
"r/w" 0x<64-bit address in Hex>. Here, "r" for read, "w" for write

The output of the simulator is statistics such as the # of hits, misses, Average Access Time etc.

The parameters - C,B,S,V,K - are provided by the user
