# jawamix5
JAWAMix5 stands for HDF5-based JAva implementation of Whole genome Association studies using Mixed model. The motivation of developing JAWAMix5 is to provide a platform-independent toolkit for mixed model-based association mapping that is scalable for very large dataset. It also supports simulation-based power estimations We intend to offer long-term maintenance for JAWAMix5 and continue adding our new developments into it.


In its first release, we provide 9 functions.

# 1. Installation

The toolkit is a batteries-included executable, therefore no installation is needed. Just copy the executable, jawamix5.jar, and run it using the standard command for java packages:

java –Xmx2g –jar /path/to/jawamix5.jar

This will prompt a help message. If that does not happen, please be so kind as to send us an email. 

# 2. Functions   

We provide ten analytical functions in version r1.1.0, the first release of JAWAMix5: 
 
(1)	An approximation of the original mixed model (Kang, Zaitlen et al. 2008), i.e., EMMAX (Kang, Sul et al. 2010));
(2)	Local variance component analysis by traditional point estimations (Yang, Benyamin et al. 2010), however jointly accounting for population structure; 
(3)	Local variance component analysis by Bayesian estimations;
(4)	Rare variants analysis using collapsing test (Li and Leal 2008) with or without population structure controlled; 
(5)	Standard linear regression without mixed model;
(6)	Standard stepwise regression without mixed model;
(7)	Stepwise regression based on mixed model;
(8)	Nested Association Mapping (NAM). (McMullen, Kresovich et al. 2009).
(9)	Simulation-based Power Estimation for the design of Rare Disease sequencing studies 


In addition to main analysis, we also provide assistant functions: 
(1)	Calculate kinship for the whole genome or particular regions;
(2)	Import the input genome files (in CSV format) to HDF5 format; 
(3)	Change the ACGT coded genotypes into number-coded genotypes and, by the way, filter out some non-qualified variants. 

# 3. Commands and options

All the functions are used as: 

```
java –Xmx2g –jar /path/to/jawamix5.jar function <options>
```
The details of the options of each function can be found in the detailed users manual.
