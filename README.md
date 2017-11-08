![My image](https://github.com/NCBI-Hackathons/Jupyter_Manifest/blob/master/Images/logo.jpg)
# Designing Educational Experiences with Jupyter Notebooks:
## A variety of NCBI Computational Tools Distributed as Jupyter Notebooks
Poor documentation leads to poor understanding of a software. It is difficult to interpret other researchers' code without unequivocal documentation. Jupyter Notebook combines code and rich-text elements which allows the user to effectively learn, modify, and run the notebook.

## Mission
The team develops tutorials explaining how to install, run, and use Jupyter Notebooks with NBCI bioinformatic tools, including tips, best practices, and examples.  The Jupyter notebooks contain live codes, equations, visualizations as well as text that can be modified and shared by users and are ideal tools to help gain familiarity with NCBI tools and data science skills.

### Project Team:
* Ray Anderson (developer)
* Richard Copin (writer / developer)
* Evgeny Ivanchenko (system admin)
* Victor Joukov (developer)
* Lon Phan (team lead)

### Directory layout

* Root
* └──[NoteBooks](/NoteBooks)               # Jupyter notebooks  
    * └──[get-list-of-genes.ipynb](/NoteBooks/get-list-of-genes.ipynb) #get list of gene features from a sequence
    * └──[Variations.ipynb](/NoteBooks/Variations.ipynb) #demos for workig with dbSNP SPDI service and JSON object
* └──Images                  # Screenshots and Presentations
* └── README.md

## Dependencies:
* Python 3 (packages such as BioPython, Macplotlib, Pandas)
* Jupyter Notebook
* Eutils Python Package
* BioPython
* XML.etree Package

### Jupyter setup instruction on your own server
Install required packages
```
pip install jupyter
pip install ipywidgets
pip install jupyter_contrib_nbextensions
pip install jupyter_nbextensions_configurator
pip install biopython
pip install requests
```
Then configure it
```
mkdir notebooks
cd notebooks/
jupyter notebook --generate-config
jupyter notebook password  # Enter your password at this step
jupyter nbextension enable --py widgetsnbextension
jupyter contrib nbextension install --user
jupyter nbextensions_configurator enable --user
```
And now run
```
jupyter notebook --no-browser --port=32888 --ip=0.0.0.0
```
Now it could be accessed by `http://localhost:32888`

### Clone and run private instance on Microsoft azure 
Click on the link below and clone the notebook into your Azure account (register free if required)
https://notebooks.azure.com/eiva/libraries/NCBInotebook

# Case Study
## Case 1
 
Disease surveillance research has led to the genome sequencing of many thousands of isolates. However, the annotation of these genome sequences is not straitghforward and often does not provide researchers with a complete set of information. Here, we present a computational pipeline to compare de novo sequence contigs to the set of complete RefSeq genomes for i) determining appropriate reference genome for whole-genome alignment, ii) proving a clean list of genes and annoated proteinsand iii) and highlitghing sets of genes invlovled in antibiotic resistance and virulence. We demonstrate our pipeline using data from S. aureus as a paradigm, owing to its high sequence variability, and therefore less well-curated genomic sequences in public databases.

![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/Images/case_study.png)




## Example screenshots

Victor Joukov  - Organism Identification from de novo reconstituted contigs
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/Images/Organism_identification.png)

Ray Anderson - EUtils Quick Start with BioPython examples
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/Images/EUtils1.png)

Evgeny Ivanchenko - List of proteins using Eutils and NCBI services (Portal, Entrez, ...)
![My image](https://github.com/NCBI-Hackathons/NCBIJupyter/blob/master/Images/gene_list.png)






