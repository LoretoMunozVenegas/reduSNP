# reduSNP
Genetic variant pruning

Introduction
reduSNP is a lightweight linkage disequilibrium (LD) pruning tool that is highlighted by it's minimum to no pre-processing of input information. It can handle large sets of SNPs with different LD threshold and uses the latest European ancestry Phase 3 realease of the 1000 Genomes Project reference population, addressing prior LD-pruning tool 'shortcomings'.

Getting started with reduSNP
The command presented here has been tested on the Ubuntu 16.04 OS runing on a x64bit machine.  This current version of reduSNP does not support Windows or Mac OS.  Future versions of the software tool may include web-based version of the tool to accommodate non-command line users.

Installation
Required software
***

Download
reduSNP command-line software package can be downloaded here (insert link)

Minimum input information
1. a list of non-ordered SNPs (rs-numbers) or InDels (e.g., rs12345)
2. a specified LD threshold(s) consisting of normalized coefficient of LD (D’) or correlation coefficient (r2) (eg. 0.8)

Running reduSNP
The basic command is:
~/redusnp.pl <input_filename>.txt <output_filename>.txt  EUR <D’ or r2 threshold(s)>
Example:  
~/folder/reduscnp.pl my_snp_list.txt results_snp_list.txt EUR 0.7 0.8 0.9 
