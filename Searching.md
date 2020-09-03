# Searching for homologous protein structures
_____
There are two approaches to retrieve protein structural data: by annotation; or by similarity.  
The choice of strategy will depend on the type of information you have at the beginning of 
your search, as well as on the problem you are trying to solve.\
The following table contains links to the main macromolecular structure resources and classification databases.

| Database                               |      | 
|----------------------------------------|------|
| [RCSB_PDB](https://www.rcsb.org/)      | Research Collaboratory for Structural Bioinformatics PDB |
| [PDBe](https://www.ebi.ac.uk/pdbe/)    | Protein Data Bank in Europe                              |
| [PDBj](https://pdbj.org/)              | Protein Data Bank Japan                                  |
| [CATH](https://www.cathdb.info/)       | Protein Structure Classification database                |
| [SCOPe](https://scop.berkeley.edu/)    | Structural Classification of Proteins — extended         |
| [ECOD](http://prodata.swmed.edu/ecod/) | Evolutionary Classification of Protein Domains           |
_____
## Exercise 1: searching by annotation (information-driven search approach) 
**Goal:** The goal of this exercise is to learn how to obtain a list of pdb entries of proteins that have a homologous domain.

**1. Go to [PDBe](https://www.ebi.ac.uk/pdbe/) and type "hemerythrin" in the search bar.** \
   This will display a menu with automated suggestions for filters that can be applied to your search. \
   In this example, there are three filters for "hemerythrin": 
   - **Molecule name** \
     This filter will allow you to retrieve all molecules annotated as "hemerytrin". \
     Two notes of caution, though. Not all homologues have the same molecular name and not al molecules with the same name are homologues.
   - **Sequence family** \
     This will filter entries by unique identifier within [Rfam](https://rfam.xfam.org/), [Pfam](https://pfam.xfam.org/) or [Interpro](https://www.ebi.ac.uk/interpro/) databases. Proteins classified within the same *family* in these databases are considered homologs.
   - **Structure domain** \
     Here you will find entries with the same [CATH](https://www.cathdb.info/) *topology*, which includes non-homologous proteins.

   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Hemerythrin_seq_fam_searchPDBe.png)

**2. Select the results for [Sequence family : PF01814 : Hemerythrin](https://www.ebi.ac.uk/pdbe/entry/search/index/?searchParams=%7B%22q_all_sequence_family%22:%5B%7B%22value%22:%22PF01814%20:%20Hemerythrin%22,%22condition1%22:%22AND%22,%22condition2%22:%22Contains%22%7D%5D,%22resultState%22:%7B%22tabIndex%22:0,%22paginationIndex%22:1,%22perPage%22:%2210%22,%22sortBy%22:%22Sort%20by%22%7D%7D).** \
   This page will display all entries associated with the Hemerythrin family in Pfam. \
   Note that the same UniProt/PDBe-KB identifier may appear in different PDB entries. \
   For example: 2awc and 2awy have the same PDBe-KB identifier. \

   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Hemerythrin_entries_per_prot.png)

**3. Go to the *Macromolecules* tab to see the individual entries gruped by UniProt identifier.** 

   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Molecules_tab.png)
   
   To get the results of this search in csv file format, click on the *Download* button on the top right corner of the results page. 
   - Select the data that you would like to download:
     - Macromolecule
     - PDB ID
   - Download as:
     - CSV
   Save the csv file in your working_directoy (we will use it later).
   
   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/PDBe_hemerythrin_download.png)
   
   The CSV file can be opened in a spreadsheet program (e.g. Excel) or in a text editor. \
   It should look like this:
   
   ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Homology_search_e1.png)
   
_____
   > _Got extra time? ... Explore PDBe-KB Aggregated Views of Proteins_ \
   > _Click on a PDBe-KB identifier to get a summary of structural and integrated data available for a full-length protein sequence._
   > 
   > ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/PDBeKB.png)
   >
_____

## Exercise 2: searching by  sequence similarity
**Goal:** the aim of this exercise is to show you how to possible homologs in the PDB using sequence similarity.
 
**1. Download or copy the sequence of [Bacteriohemerythrin](https://www.uniprot.org/uniprot/Q60AX2.fasta) from _Methylococcus capsulatus_.**

**2. Go to [HHpred](https://toolkit.tuebingen.mpg.de/tools/hhpred) and paste or upload the sequence of Bacteriohemerythrin**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/HHpred_sequence.png)
  
  - **Select PDB_mmCIF70_23_Jul on the *Select structural/domain databases* menu.**
    
  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/HHpred_select_options.png)
    
  - **Click the *Submit* button.**
    
  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/HHpred_submit.png)
    
   **The results may take a few minutes!** But, to save some time, we pre-calculated this search, the results can be found **[here](https://toolkit.tuebingen.mpg.de/jobs/Q60AX2)**. \
   Because we already ran this search, HHpred will display the following message when you try to do the exact same search. \
   We suggest to click the *Load existing job* button.
    
  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/HHpred_already_exists.png)

**3. Examine the results**

  ![](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/HHpred_hits.png)
     
 Compare the PDB codes of the hits list to the results obtained in the previous exercise (Information-driven search).\
 Are there results with a probability > 60% that were not retrieved using the information-driven search approach (Exercise 1)?
 How many new PDB codes did we obtain during this similarity search approach?

**We will analize some of these results in the next sections.**

## Further reading
> Fitch WM. Homology a personal view on some of the problems.  
Trends Genet. 2000;16(5):227-231. doi:10.1016/s0168-9525(00)02005-9
