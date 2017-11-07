# Designing Educational Experiences with Jupyter Notebooks:
## A variety of NCBI Computational Tools Distributed as Jupyter Notebooks
Poor documentation leads to poor understanding of a software. It is difficult to interpret other researchers' code without unequivocal documentation. Jupyter Notebook combines code and rich-text elements which allows the user to effectively learn, modify, and run the notebook.

### directory layout

    .
    ├── NoteBooks               # Jupyter notebooks
    ├── Scripts                 # Scripts and tutorials
    ├── Images
    └── README.md

## Dependencies:
* Python 3 (packages such as BioPython, Macplotlib, Pandas)
* Jupyter Notebook
* Eutils Python Package
* BioPython
* XML.etree Package

# Case Study
## Case 1
 
Disease surveillance research has led to the genome sequencing of many thousands of isolates. However, the annotation of these genome sequences is not straitghforward and often does not provide researchers with a complete set of information. Here, we present a computational pipeline to compare de novo sequence contigs to the set of complete RefSeq genomes for i) determining appropriate reference genome for whole-genome alignment, ii) proving a clean list of genes and annoated proteinsand iii) and highlitghing sets of genes invlovled in antibiotic resistance and virulence. We demonstrate our pipeline using data from S. aureus as a paradigm, owing to its high sequence variability, and therefore less well-curated genomic sequences in public databases.

![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/case_study.png)


### Project Team:
* Ray Anderson (developer)
* Richard Copin (writer / developer)
* Evgeny Ivanchenko (system admin)
* Victor Joukov (developer)
* Lon Phan (team lead)

## Example screenshots

Victor Joukov  - Organism Identification from de novo reconstituted contigs
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/Organism_identification.png)

Ray Anderson - EUtils Quick Start with BioPython examples
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/EUtils1.png)

Evgeny Ivanchenko - List of proteins using Eutils and NCBI services (Portal, Entrez, ...)
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/gene_list.png)






