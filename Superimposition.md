## Overview of pairwise structure superimposition tools:

Wikipedia has a list of many avaliable structural alignment programs: https://en.wikipedia.org/wiki/Structural_alignment_software \
In this tutorial we will use only a few of them.

| Name          | Description   | Type  |
| ------------- |---------------| ------|
| [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) | TM-score based protein structure alignment | sequential |
| [CE](http://www.rcsb.org/pdb/workbench/workbench.do)      | Combinatorial Extension | sequential |
| [DALI](http://ekhidna2.biocenter.helsinki.fi/dali/) | Distance‐matrix ALIgnment | non-sequential* |
| [MICAN](http://www.tbp.cse.nagoya-u.ac.jp/MICAN/index.html)   | Multiple-chains, Inverse alignments, C α only models, Alternative alignments, and Non-sequential alignments | non-sequential |
| [CLICK](http://cospi.iiserpune.ac.in/click/) | Topology-independent 3D structure comparison | non-sequential |
| [Rapido](http://rapido.embl-hamburg.de/) | Rapid Alignment of Protein structures In the presence of Domain mOvements | sequential, flexible |
| [MetalS2](http://metalweb.cerm.unifi.it/tools/metals2/)| Pairwise structural alignment of Minimal Functional Sites in metal-binding biological macromolecules | non-sequential, other |

Let's start by aligning two structures that share a homologous domain.
1. Download the PDB coordinates files of [Bacteriohemeritrin](http://www.rcsb.org/structure/4XPX) from _Methylococcus capsulatus str. Bath_ and the [Hypothetical protein NMB1532](http://www.rcsb.org/structure/2P0N) from _Neisseria meningitidis MC58_ and save them in your working_directory. \

Go to the [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) web server page. \

3. Inspect the results. \
TM-align will output 
`` \
 ************************************************************************** \
 *                        TM-align (Version 20190822)                     * \
 * An algorithm for protein structure alignment and comparison            * \
 * Based on statistics:                                                   * \
 *       0.0 < TM-score < 0.30, random structural similarity              * \
 *       0.5 < TM-score < 1.00, in about the same fold                    * \
 * Reference: Y Zhang and J Skolnick, Nucl Acids Res 33, 2302-9 (2005)    * \
 * Please email your comments and suggestions to: zhng@umich.edu          * \
 ************************************************************************** \
``
 Name of Chain_1: A103021                                           
 Name of Chain_2: B103021                                           
 Length of Chain_1:  130 residues
 Length of Chain_2:  157 residues
 
 Aligned length=  116, RMSD=   3.38, Seq_ID=n_identical/n_aligned= 0.103
 TM-score= 0.62196 (if normalized by length of Chain_1)
 TM-score= 0.53857 (if normalized by length of Chain_2)
 (You should use TM-score normalized by length of the reference protein)
 
 (":" denotes aligned residue pairs of d < 5.0 A, "." denotes other aligned residues)
 ALMTWTAAEFGTN-----VGFADDQHKTIFDMVNKLHDTAAT----GN--RSEIGKQLDALID-YVVMHFKSEETEMQKKGY------AD-FAAHKAEHDKLVGVCADLQKKFHA--G---EAEVNQDTTRFVRDWLVNHIPKVDKLYGPCLSA-----------------
                   .::::::::::::::::::...::    ::  .:::::::::::: ::::::::::::::::.:      :: ::::::::::::::::::::::::  .   ..:.. .::::::::::::::::::::::...:                 
 -------------VTFAEPIELYACHGKVRRFCGQVALSDYIAENGCNQIVLQTIRQIAQYFNVAAPLHHEDEEENFFPLLLQYAPQAQESVDELLRQHIGLHDNWAAVSAEFAKLEADNAYVPDE-EAFKRFVAGYDVHLAIEEPLFDGNTFIPKEKLTEIGEIAARRRK


 


_______
## Further reading

> Joung I, Kim JY, Joo K, Lee J. Non-sequential protein structure alignment by conformational space annealing and local refinement. PLoS One. 2019;14(1):e0210177. Published 2019 Jan 30. doi:10.1371/journal.pone.0210177

> Zhang Y, Skolnick J. TM-align: a protein structure alignment algorithm based on the TM-score. Nucleic Acids Res. 2005;33(7):2302-2309. Published 2005 Apr 22. doi:10.1093/nar/gki524

> Xu J, Zhang Y. How significant is a protein structure similarity with TM-score = 0.5?. Bioinformatics. 2010;26(7):889-895. doi:10.1093/bioinformatics/btq066
