# Introduction to web tools for protein structure classification
_____
The Protein Data Bank (PDB, pdb.org) is the unique repository of atomic coordinate files and other information about nucleic acids, proteins and complexes. Each coordinate file consists of a list of atoms in each structure and their 3D location in space.
 
The PDB is managed jointly by the World- wide Protein Data Bank (wwPDB) consortium and is conformed by many members all around the world, in-cluding the US Research Collaboratory for Structural Bioinformatics Protein Data Bank ([RCSB PDB](https://www.rcsb.org/)), the Protein Data Bank in Europe ([PDBe](pdbe.org)), Protein Data Bank Japan ([PDBj](pdbj.org)) and BioMagResBank ([BMRB](www.bmrb.wisc.edu)).


_____
## Exercise 1: Protein Data Bank (PDB) exploration

Goal: Search for structural data in PDB and explore the available information for the protein of interest. This exercise will be focused on how to identify the pfam architecture, the secondary structure content, found the links to the domain classification databases (CATH and SCOP) and visualize the tridimensional structures of protein domains.

1. Go to the [PDBe](https://www.ebi.ac.uk/pdbe/) site and in the "search" upper right green icon, write "Hemerythrin". 

![hemerythrinsearch.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/hemerythrinsearch.png?raw=true)

2. Search in the "Macromolecules" section in the upper left side and click on the "Organism superkingdom", then select "Archaea".

![Macromolecules.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Macromolecules.png?raw=true)

3. Click on the structure [3cax](https://www.ebi.ac.uk/pdbe/entry/pdb/3cax).
4. In the main page, you will find the grey box "Structure analysis" in the lower right side. Click on [Molecule details](https://www.ebi.ac.uk/pdbe/entry/pdb/3cax/protein/1).

![Macromolecules.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Macromolecules.png?raw=true)

5. Locate the middle section "Visualisation". Find the "Pfam" row and signal the domain "Hemerythrin HHE cation binding domain". Observe that in the visualizer your that domain is now highlighted in pink. Identify the regions of the domain (9-148).

![Macromolecules.png](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/Macromolecules.png?raw=true)


6. Find the "Sec. str" section.
7. In the "CATH" section, you will see that your domain correspond to the CATH superfamily (1.20.120.520)[http://www.cathdb.info/version/latest/superfamily/1.20.120.520]. 

![3cax_visualization_domain_pdbe](https://github.com/Claualvarez/ECCB2020/blob/master/Figures/3CAX_domainpdbeCATH.png?raw=true)


Note: Although you can use the PDB visualization system, you can also explore all the (Molecular Graphics Software programs)[https://www.rcsb.org/pages/thirdparty/molecular_graphics].


_______
## Exercise 2: Retrieving structural data from PDB

Goal: Download atomic coordinate files from the PDB.

Is time to download the atomic coordinate file of our protein of interest
1. Go to the main page of the structure [3cax](https://www.ebi.ac.uk/pdbe/entry/pdb/3cax).
2. In the upper-right box "Quick links", find the section "Downloads". Click on the "PDB file" blue link.
3. Direct to your Download section and open the file "pdb3cax.ent" with the editor of your computer.




_______
## Further reading
>  Berman H, Westbrook J, Feng Z, Gilliland T, Bhat T, Weissig H, Shindyalov I, Bourne P. The Protein Data Bank. Nucleic Acids Research. 2000. 28: 235-242. doi:10.1093/nar/28.1.235.

>  Berman H, Westbrook J, Feng Z, Gilliland T, Bhat T, Weissig H, Shindyalov I, Bourne P. The Protein Data Bank. Nucleic Acids Research. 2000. 28: 235-242. doi:10.1093/nar/28.1.235. PDB101.rcsb.org.

>  Velankar, S., Alhroub, Y., Alili, A., Best, C., Boutselakis, H. C., Caboche, S., Conroy, M. J., Dana, J. M., van Ginkel, G., Golovin, A., Gore, S. P., Gutmanas, A., Haslam, P., Hirshberg, M., John, M., Lagerstedt, I., Mir, S., Newman, L. E., Oldfield, T. J., Penkett, C. J., … Kleywegt, G. J. (2011). PDBe: Protein Data Bank in Europe. Nucleic acids research, 39(Database issue), D402–D410. https://doi.org/10.1093/nar/gkq985https://www.ebi.ac.uk/pdbe/training.







