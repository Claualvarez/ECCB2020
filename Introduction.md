
17.00 – 17.40

Introduction to web tools for protein structure classification 

1. Globular and elongated domains


2.  Intrinsically disordered proteins and regions


3. Introduction to data file formats: PDB and mmCIF 

The PDB archive is a repository of atomic coordinates and other information describing proteins and other important biological macromolecules. Structural biologists use methods such as X-ray crystallography, NMR spectroscopy, and cryo-electron microscopy to determine the location of each atom relative to each other in the molecule. They then deposit this information, which is then annotated and publicly released into the archive by the wwPDB.

PDB Data
The primary information stored in the PDB archive consists of coordinate files for biological molecules. These files list the atoms in each protein, and their 3D location in space. These files are available in several formats (PDB, mmCIF, XML). A typical PDB formatted file includes a large "header" section of text that summarizes the protein, citation information, and the details of the structure solution, followed by the sequence and a long list of the atoms and their coordinates. The archive also contains the experimental observations that are used to determine these atomic coordinates.

For all PDB entries, the file https://cdn.rcsb.org/etl/kabschSander/ss_dis.txt.gz notes regions of the molecule that have not been observed (e.g. residues which exist in the originally studied molecule as shown in the SEQRES records, but not in the observed structure/coordinates).


Activity: Retrieving PDB files of your protein of interest

Go to PDB database and search for the protein structure “1DMG”.
https://www.rcsb.org/structure/1DMG

Click in the “Download files” section and select “PDB format” and “PDBx/mmCIF”.




Useful links:


An initial guide to understanding PDB database

https://pdb101.rcsb.org/learn/guide-to-understanding-pdb-data/beginner%E2%80%99s-guide-to-pdb-structures-and-the-pdbx-mmcif-format

A friendly site to download PDB files in a high-throughput scale
Description: PDB entry files, chemical component files, and other data files are available for Display and/or Download via http and https. These URLs are useful with scripted downloads using utilities such as wget.

https://www.rcsb.org/pdb/static.do?p=download/http/index.html

SIFTS project: updated mapping between UniProt and PDB
Structure Integration with Function, Taxonomy and Sequence (SIFTS) is a project in the PDBe-KB resource for residue-level mapping between UniProt and PDB entries. SIFTS also provides annotation from the IntEnz, GO, InterPro, Pfam, CATH, SCOP, PubMed, Ensembl and Homologene resources. The information is updated and released every week concurrently with the release of new PDB entries and is widely used by resources such as RCSB PDB, PDBj, PDBsum, Pfam, SCOP and InterPro.

https://www.ebi.ac.uk/pdbe/docs/sifts/quick.html

PDB bundle: a repository for huge PDB files
Due to the size of the large structures, they are not compatible with the legacy pdb format. For this reason these entries are only released using the PDBx/mmCIF and PDBML formats. However, since many legacy software still cannot properly load the PDBx/mmCIF or PDBML format, the wwPDB has created a bundle of best-effort pdb files. Here, the data for the large structures is split over multiple pdb files and combined into a single bundle. Also included is a mapping file (****-chain-id-mapping.txt) to map the chain ids as given in each of the bundles to the originally assigned chain id as found in the PDBx/mmCIF and PDBML files.

https://pdbj.org/help/pdb-bundle


