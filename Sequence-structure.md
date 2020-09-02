# Correspondences between protein sequence and structure
_____
In the 1960s, Christian Anfinsen postulated that the unique three-dimensional structure of a protein is determined by its amino acid sequence (sequence–structure–function paradigm). However, there are some exceptions, intrinsically disordered proteins and regions does not conform to this postulate. Disordered regions contribute to protein function and do not fold into a defined tertiary structure.

Protein structure prediction techniques fall into two main categories: Template-free (or de novo) and Template-based (or homology-modeling). The first one do not use any known structures. Useful when not a single structure in a protein family is known. Whereas the Template-based employ the similarity to another protein whose three-dimensional structure is known. 

Whereas there exist many Protein structure predictors, Intrinsically Disordered Proteins (IDPs) and Intrinsically Disordered  Regions (IDRs) can be inferred by the amino acid sequence. The distinct sequence features that are present in IDPs and IDRs allow the construction of sequence based rules that can facilitate high performance disorder prediction.

_______
## Exercise 1: Template-based structure prediction
 
 
 
 
_______
## Exercise 2: Intrinsically disordered regions prediction

Predict intrinsically disordered regions in our protein of interest
1. Prepare the fasta sequence of your protein of interest. If you´re interested in predict the disorder in a PDB entry, go to the main page [1zr9](https://www.ebi.ac.uk/pdbe/entry/pdb/1zr9).
2. In the main page, you will find the grey box "Structure analysis" in the lower right side. Click on [Molecule details](https://www.ebi.ac.uk/pdbe/entry/pdb/1zr9/protein/1). In the upper gray box, identify the term "UniProt:" and copy the code (O00488).
3. Go to the [UniProt site](https://www.uniprot.org/) and search fot the UniProt code (O00488)[https://www.uniprot.org/uniprot/O00488]. Search for the (fasta sequence)[https://www.uniprot.org/uniprot/O00488.fasta] and copy it in the text editor installed in your computer.
4. Direct to the (IUPred2A)[https://iupred2a.elte.hu/], an intrinsic disordered predictor.
5. Paste your amino acid fast sequence in the central white box. Click on submit. Be sure that the option "IUPred2 long disorder (default)" is selected.
6. Visualize your disorder prediction results. In the graph you can see the disorder prediction with the red line. All those residues in the positions that have values with a score >0.5, are considered as disordered. You can also download your results in "Text" or "JSON" formats in the "Download results" upper icon.
 
 ![IUPredlong results](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/iupred_graphO00488results.png?raw=true)

7. Search for your protein with their UniProt code "O00488" in the (DisProt database)[https://www.disprot.org/]. 
8. Explore all the available experimental information and disorder biological information related with your (protein)[https://www.disprot.org/DP00549?release=current&show_ambiguous=true&show_obsolete=false].

 ![IUPredlong results](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/DisProt_O00488.png?raw=true)
 

_______
## Further reading
 












