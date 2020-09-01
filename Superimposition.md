## Overview of pairwise structure superimposition tools:

Wikipedia has a list of [structural alignment programs](https://en.wikipedia.org/wiki/Structural_alignment_software). \
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
## Exercise 1: 4xpx vs. 2p0n
Let's start by superimposing the structure of Bacteriohemerythrin to 2p0n, a possible homolog that we identified using [HHpred](https://github.com/Claualvarez/ECCB2020/blob/master/Searching.md).

**1. Download the PDB coordinates files of [Bacteriohemeritrin](https://www.ebi.ac.uk/pdbe/entry/pdb/4xpx/) from _Methylococcus capsulatus str. Bath_ and the [Hypothetical protein NMB1532](https://www.ebi.ac.uk/pdbe/entry/pdb/2p0n) from _Neisseria meningitidis MC58_ and save them in your working_directory.** 

**2. Go to the [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) web server page and upload the two PDB files that you just downloaded.**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TM-align.png)
  
  Click on *Run TM-align* to start the superimposition.
  
  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TM-align_run.png)
  
**3. Examine and save the [results](https://zhanglab.ccmb.med.umich.edu/TM-align/tmp/103021.html).** 
  
  - The first part of the output contains the `Aligned length`, `RMSD`, `Seq_ID` (proportion of identical positions to aligned residues), and `TM-score`.\
    How many residues have been aligned? \
    What is the TM-score of this superimposition? \
    What is the RMSD of this superimposition?
    
  - Next, you will see the structure-derived sequence alignment.
     
     > *Tip:* \
     > Always examine the structure-derived sequence alignment. \
     > The structure-derived sequence alignment can be easily converted to a FASTA format using a text editor (or with a parsing script). \
     > Just remeber: \
     >   (":" denotes aligned residue pairs of d < 5.0 A, "." denotes other aligned residues) \
     > You can use the sequence alignment to seed a multiple sequence alignment (we will do this in the next session).
  
    ![TM-align output for the alignment of 4xpx:A and 2p0n:A](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_output.png?raw=true)

  - TM-align displays the structure superimposition of the two macromolecules. 

    ![TM-align structure superimposition](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_output-visualization.png)
  
  - Finally, TM-align outputs a set of PDB files of the structure superimposition. 
  
_______
## Exercise 2: 4xpx vs. 5fnn 
For the second exercise we will use a different pair of proteins that have a homologous domain.

**1. Download the PDB coordinates file of [YtfE](https://www.ebi.ac.uk/pdbe/entry/pdb/5fnn) from _Escherichia coli K-12_ and save it in your working_directory.**

**2. Go to the [TM-align](https://zhanglab.ccmb.med.umich.edu/TM-align/) web server page and upload the PDB file for 4xpx and 5fnn and run the superimposition by clicking the *Run TM-align* button.** 

**3. Examine the [results](https://zhanglab.ccmb.med.umich.edu/TM-align/tmp/115059.html).**

  ![TM-align output for the alignment of 2p0n:A and 5fnnA](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/TMalign_2p0n-5fnn_output.png)

  How many residues have been aligned? \
  What is the TM-score of this superimposition? \
  What is the RMSD of this superimposition?
    
**4. Let's try a different algorithm. Go to the [CLICK web server](http://cospi.iiserpune.ac.in/click/).** 

**5. Upload the files or provide the pdb codes of the proteins that we want to compare (4xpx and 5fnn).**

**6. Run the alignment or click [here](http://cospi.iiserpune.ac.in/click/output/01092020233149/01092020233149.html) to open the pre-computed superimposition.**

**7. Examine the results and compare them to the superimposition coputed with TM-align. \
Locate the alignment summary.**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/CLICK_summary.png)
  
**Pay particular attention to the structure-derived sequence alignment.**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/CLICK_seq_aln.png)
  
  How many residues have been aligned? \
  What is the RMSD of this superimposition?
  
**Are these superimpositions substantially different? Why? And how do you decide which one to use?**

_______
## Further reading

> Joung I, Kim JY, Joo K, Lee J. Non-sequential protein structure alignment by conformational space annealing and local refinement. PLoS One. 2019;14(1):e0210177. Published 2019 Jan 30. doi:10.1371/journal.pone.0210177

> Zhang Y, Skolnick J. TM-align: a protein structure alignment algorithm based on the TM-score. Nucleic Acids Res. 2005;33(7):2302-2309. Published 2005 Apr 22. doi:10.1093/nar/gki524

> Xu J, Zhang Y. How significant is a protein structure similarity with TM-score = 0.5?. Bioinformatics. 2010;26(7):889-895. doi:10.1093/bioinformatics/btq066
