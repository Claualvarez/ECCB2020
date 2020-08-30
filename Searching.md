# Searching for homologous protein structures
_____
There are two approaches to retrieve protein structural data: by annotation; or by similarity.  
The choice of strategy will depend on the type of information you have at the beginning of 
your search, as well as on the problem you are trying to solve.

#### The Protein Data Bank database
[RCSB_PDB](https://www.rcsb.org/); [PDBe](https://www.ebi.ac.uk/pdbe/); [PDBj](https://pdbj.org/)
#### Structure classification databases
- [CATH](https://www.cathdb.info/); 
- [SCOPe](https://scop.berkeley.edu/); 
- [ECOD](http://prodata.swmed.edu/ecod/)


_____
## Exercise 1: searching by annotation (information-driven search approach) 

**1. Go to [PDBe](https://www.ebi.ac.uk/pdbe/) and type "hemerythrin" in the search bar.** \
   This will display results for "hemerythrin" in three categories: 
   - **Molecule name**: 
     This filter will allow you to retrieve all molecules annotated as "hemerytrin". \
     Two notes of caution, though. Not all homologues have the same molecular name and not al molecules with the same name are homologues.
   - **Sequence family**:
     This will filter -at the *family* level- entries by unique identifier within [Rfam](https://rfam.xfam.org/), [Pfam](https://pfam.xfam.org/) or [Interpro](https://www.ebi.ac.uk/interpro/) databases. Proteins classified within the same *family* in these databases are considered homologs.
   - **Structure domain**:
     Here you will find entries with the same [CATH](https://www.cathdb.info/) *topology*, which includes non-homologous proteins.

   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Hemerythrin_seq_fam_searchPDBe.png)

**2. Select the results for Sequence family : PF01814 : Hemerythrin.** \
   This page will display all entries associated with the Hemerythrin family in Pfam. \
   Note that the same [UniProt](https://www.uniprot.org/)/PDBe-KB identifier may appear in different PDB entries. \
   For example: 2awc and 2awy have the same PDBe-KB identifier. 

   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Hemerythrin_entries_per_prot.png)

**3. Go to the *Macromolecules* tab to see the individual entries gruped by [UniProt](https://www.uniprot.org/) identifier.** 
   To get the results of this search in csv file format, click on the *Download* button on the top right corner of the results page. 
   - Select the data you would like to download:
     - Macromolecule
     - PDB ID
   - Download as:
     - CSV
   Save the csv file in your working_directoy (we will use it later).
_____
   > Got extra time? ... Explore PDBe-KB Aggregated Views of Proteins \
   > Click on a PDBe-KB identifier to get a summary of structural and integrated data available for a full-length protein sequence.
   > 
   > ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/PDBeKB.png)
   >
_____

## Exercise 2: searching by  sequence similarity
 
**1. Download the sequence of [Bacteriohemerythrin](https://www.uniprot.org/uniprot/Q60AX2.fasta) from _Methylococcus capsulatus_**
  - [HHpred](https://toolkit.tuebingen.mpg.de/tools/hhpred)
- By structure similarity: 
  - [PDBeFold](https://www.ebi.ac.uk/msd-srv/ssm/) 
  - [DALI - PDB search](http://ekhidna2.biocenter.helsinki.fi/dali/)

## Further reading
> Fitch WM. Homology a personal view on some of the problems.  
Trends Genet. 2000;16(5):227-231. doi:10.1016/s0168-9525(00)02005-9
