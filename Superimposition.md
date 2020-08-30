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


_______
## Exercise 1
Let's start by aligning two structures that share a homologous domain.
1. Download the PDB coordinates files of [Bacteriohemeritrin](https://www.ebi.ac.uk/pdbe/entry/pdb/4xpx/) from _Methylococcus capsulatus str. Bath_ and the [Hypothetical protein NMB1532](https://www.ebi.ac.uk/pdbe/entry/pdb/2p0n) from _Neisseria meningitidis MC58_ and save them in your working_directory. 

2. Go to the [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) web server page. 

3. Interpreting the [results](https://zhanglab.ccmb.med.umich.edu/TM-align/tmp/103021.html). 
  - The first part of the output contains the `Aligned length`, `RMSD`, `Seq_ID` (proportion of identical positions to aligned residues), and `TM-score`.
  - Next, the structure-derived sequence alignment, which can be easily converted to a FASTA format using a text editor (or with a parsing script).
  Once you have added a name for each sequence, the structure-derived fasta alignment will look like [this](https://github.com/Claualvarez/ECCB2020/blob/master/Files/4xpxA-2p0nA.tmalign_aln.fa).
     - Always examine the structure-derived sequence alignment. 
     - You can use the sequence alignment to seed a multiple sequence alignment (we will do this in the next session).
  
![TM-align output for the alignment of 4xpx:A and 2p0n:A](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_output.png?raw=true)

  - TM-align displays the structure superimposition of the two macromolecules. 

![TM-align structure superimposition](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_output-visualization.png)
  - PDB files
  
_______
## Exercise 2
For the second exercise we will use a different pair of proteins that have a homologous domain.

1. Download the PDB coordinates file of [YtfE](http://www.rcsb.org/structure/5FNN) from _Escherichia coli K-12_ and save it in your working_directory.

2. Go to the [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) web server page. 

3.

![TM-align output for the alignment of 2p0n:A and 5fnnA](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_2p0n-5fnn_output.png)
_______
## Further reading

> Joung I, Kim JY, Joo K, Lee J. Non-sequential protein structure alignment by conformational space annealing and local refinement. PLoS One. 2019;14(1):e0210177. Published 2019 Jan 30. doi:10.1371/journal.pone.0210177

> Zhang Y, Skolnick J. TM-align: a protein structure alignment algorithm based on the TM-score. Nucleic Acids Res. 2005;33(7):2302-2309. Published 2005 Apr 22. doi:10.1093/nar/gki524

> Xu J, Zhang Y. How significant is a protein structure similarity with TM-score = 0.5?. Bioinformatics. 2010;26(7):889-895. doi:10.1093/bioinformatics/btq066
