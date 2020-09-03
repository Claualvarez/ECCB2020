## Exercise 1: From structure to sequence
**Goal:** In this exercise we will use the list of pdb entries that are classified as Hemerythrin according to Pfam (Pfam code: PF01814). \
We will use one pdb code per macromolecule. \
This is the **[list](https://www.ebi.ac.uk/pdbe/entry/search/index/?searchParams=%7B%22q_all_sequence_family%22:%5B%7B%22value%22:%22PF01814%20:%20Hemerythrin%22,%22condition1%22:%22AND%22,%22condition2%22:%22Contains%22%7D%5D,%22resultState%22:%7B%22tabIndex%22:1,%22paginationIndex%22:1,%22perPage%22:%2210%22%7D%7D)** of pdb codes that we will use:
- 4xpyA
- 3v5xA
- 6tyjA
- 3agtA
- 1a7dA

> *We will exclude from this search all pdb extries related to the Iron-sulfur cluster repair protein YtfE (5fnn, 5fny, 5fnp) and pdb entries related to the Uncharacterized protein PF0695 (3cax). These proteins are structurally different. If we want to include them in a multiple structure alignment, further refinement steps are required.*

**1. Go to the [MATRAS](http://strcomp.protein.osaka-u.ac.jp/matras/) web page.** \
We want to calculate a Multiple Sequence Alignment. On the menu, locate the [Multiple 3D Alignment link](http://strcomp.protein.osaka-u.ac.jp/matras/matras_multi.html), and click to go to the algorithm page. 
  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/MATRAS_homepage.png)

**2. Enter one representative pdb code per macromolecule.**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/MATRAS_input_C.png)

**3. Examine the results.**
Matras outputs a structure-based multiple sequence alignment in a special file format. \
We have transformed this multiple sequence alignment into a [fasta file format](https://github.com/Claualvarez/ECCB2020/blob/master/Files/hemerythrin_rep_seqs.matras.fa). 
These proteins are very distantly related! Hemerytrins and hemerythrin-like domains form a large and diverse superfamily of folds. \
Only a few amino acid positions are conserved.

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/MATRAS_output_C.png)
  
**4. Download and examine the *trimmed* [fasta file format](https://github.com/Claualvarez/ECCB2020/blob/master/Files/hemerythrin_rep_seqs.matras.trimmed.fa) of the multiple sequence alignment that we calculated using matras.**

**What can we do with this structue-based multiple sequence alignment?**
- Search homologous sequences in [hhblits](https://toolkit.tuebingen.mpg.de/jobs/hemerythrin).
- Seed and refine a multiple sequence alignment using, for example, [mafft add](https://mafft.cbrc.jp/alignment/server/add.html)
  - Use this refined MSA to calculate a phylogeny.
- [Visualize the conservation of the amino acid residues using consurf](https://consurf.tau.ac.il/fgij/fg.htm?mol=/results/1599141144/4xpy_consurf1599141144_pipe_CBS.pdb). 
_____
## Further reading
> Kovacs NA, Penev PI, Venapally A, Petrov AS, Williams LD. Circular Permutation Obscures Universality of a Ribosomal Protein. J Mol Evol. 2018;86(8):581-592. doi:10.1007/s00239-018-9869-1

> Grishin NV. Fold change in evolution of protein structures. J Struct Biol.
> 2001;134(2-3):167-185. doi:10.1006/jsbi.2001.4335

