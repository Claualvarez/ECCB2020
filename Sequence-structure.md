# Correspondences between protein sequence and structure
_____
In the 1960s, Christian Anfinsen postulated that the unique three-dimensional structure of a protein is determined by its amino acid sequence (sequence–structure–function paradigm). However, there are some exceptions, intrinsically disordered proteins and regions does not conform to this postulate. Disordered regions contribute to protein function and do not fold into a defined tertiary structure.

Protein structure prediction techniques fall into two main categories: Template-free (or de novo) and Template-based (or homology-modeling). The first one do not use any known structures. Useful when not a single structure in a protein family is known. Whereas the Template-based employ the similarity to another protein whose three-dimensional structure is known. 

Whereas several protein structure predictors, Intrinsically Disordered Proteins (IDPs) and Intrinsically Disordered  Regions (IDRs) also can be inferred by the amino acid sequence. The distinct sequence features that are present in IDPs and IDRs allow the construction of sequence based rules that can facilitate high performance disorder prediction.

_______
## Exercise 1: Template-based structure prediction

Goal: Predict a protein structure by homology modeling methods, based on the sequence similarity to another protein whose three-dimensional structure is determined.

1. Go to the (SWISS-MODEL)[https://swissmodel.expasy.org/interactive] site. 
2. Access to the (UniProt site)[https://www.uniprot.org/] and search the code ("Q0PC81")]. This is the protein you will model, the hemerythrin of Campylobacter jejuni.
3. Go back to the (SWISS-MODEL)[https://swissmodel.expasy.org/interactive] site and paste the code "Q0PC81" (without quotation marks) in the "Target Sequence(s)" space.

![swissmodel.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/swissmodel.png?raw=true)

![swissmodel.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/uniprotsequencesp.png?raw=true)

4. Add a title to your project, name it "Hemerythrin" and append your email (optional).
5. Click on the left blue button "Search for templates". The templates search will use (BLAST)[https://blast.ncbi.nlm.nih.gov/Blast.cgi] and (HHblits)[.de/tools/hhblits]. Wait for some minutes.

 ![waitswissmodel.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/waitswissmodel.png?raw=true)

6. The results of the templates will be listed together with some relevant structural information. Select the code "4xpw.1.A". Click on the arrow at the the left of side and it will appear a description of the template of your selection.

 ![templateswissmodel.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/templateswissmodel.png?raw=true)

7. Click on the blue button "Build model". Once your model has been done, click on the upper blue button "Build models"

 ![modeltemplateswissmodel.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/modeltemplateswissmodel.png?raw=true)
 
 


Note: We recommend you to read the help section of (SWISS-MODEL)[https://swissmodel.expasy.org/docs/help#new_project] to obtain detailed information.


_______
## Exercise 2: Intrinsically disordered regions prediction

Goal: Predict disordered regions from a fasta sequence and get familiarized with the common output format of disordered predictors.

1. Prepare the fasta sequence of your protein of interest. If you´re interested in predict the disorder in a PDB entry, go to the main page [1zr9](https://www.ebi.ac.uk/pdbe/entry/pdb/1zr9).
2. In the main page, you will find the grey box "Structure analysis" in the lower right side. Click on [Molecule details](https://www.ebi.ac.uk/pdbe/entry/pdb/1zr9/protein/1). In the upper gray box, identify the term "UniProt:" and copy the code (O00488).
3. Go to the [UniProt site](https://www.uniprot.org/) and search fot the UniProt code (O00488)[https://www.uniprot.org/uniprot/O00488]. Search for the (fasta sequence)[https://www.uniprot.org/uniprot/O00488.fasta] and copy it in the text editor installed in your computer.
4. Direct to the (IUPred2A)[https://iupred2a.elte.hu/], an intrinsic disordered predictor.
5. Paste your amino acid fast sequence in the central white box. Click on submit. Be sure that the option "IUPred2 long disorder (default)" is selected.
6. Visualize your disorder prediction results. In the graph you can see the disorder prediction with the red line. All those residues in the positions that have values with a score >0.5, are considered as disordered. You can also download your results in "Text" or "JSON" formats in the "Download results" upper icon.
 
 ![IUPredlong results](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/iupred_graphO00488results.png?raw=true)

7. Search for your protein with their UniProt code "O00488" in the (DisProt database)[https://www.disprot.org/]. 
8. Explore all the available experimental information and disorder biological information related with your (protein)[https://www.disprot.org/DP00549?release=current&show_ambiguous=true&show_obsolete=false].

 ![DisProt_O00488](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/DisProt_O00488.png?raw=true)
 

_______
## Further reading
>  Necci M​,  Piovesan D,​ CAID Predictors ​, DisProt Curators ​. Tosatto S. Critical Assessment of Protein Intrinsic Disorder Prediction.  doi:10.1101/2020.08.11.245852.
> van der Lee et al. Classification of Intrinsically Disordered Regions and Proteins.  Chem. Rev. 2014. 114: 6589−6631. doi:10.1021/cr400525. 

















