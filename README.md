# BOOM Speculative Attacks

This repository holds all the work-in-progress code used to check if BOOM is susceptible to Spectre attacks.

# Project Members

| Name             | Github Handle |
| ---------------- | ------------- |
| Abraham Gonzalez | abejgonzalez  |
| Ed Younis        | riyt          |
| Ben Korpan       | bkorpan       |
| Jerry Zhao       | jerry123      |


## Implemented Attacks

The following attacks are implemented within the repo.

* Spectre-v1 or Bounds Check Bypass [1]
    * condBranchMispred.c
* Spectre-v2 or Branch Target Injection [1]
    * indirBranchMispred.c

## Not Completed Attacks

The following attacks are in-progress and are not working yet.

* Return Stack Buffer Attack [2]
    * returnStackBuffer.c
    * Main reason why this doesn't work is because the RSB was disconnected in the BPU (commented out). 

# Building the tests

To build you need to run `make`

# Running the Tests

This builds "baremetal" binaries that can directly run on the BOOM configuration that was specified above.

# References

[1] P. Kocher, D. Genkin, D. Gruss, W. Haas, M. Hamburg, M. Lipp, S. Mangard, T. Prescher, M. Schwarz, and Y. Yarom, “Spectre attacks: Exploiting speculative execution,” ArXiv e-prints, Jan. 2018

[2] E. M. Koruyeh, K. N. Khasawneh, C. Song, N. Abu-Ghazaleh, “Spectre Returns! Speculation Attacks using the Return Stack Buffer,” 12th USENIX Workshop on Offensive Technologies, 2018
