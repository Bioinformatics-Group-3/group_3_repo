
Lab Report #1 — Open datasets regarding brain structure and function and the associated neurogenetics and transcriptome profiles of certain brain regions in a variety of brain disorders
Biologist: Leeva Selioutski 
Date: 10.29.25

GitHub Code: 
https://zenodo.org/record/8158914
 https://github.com/compneurobilbao/bha2/blob/main/src/build_tree.py

https://github.com/compneurobilbao/bha2/tree/main/notebooks

https://github.com/compneurobilbao/bha2 

https://zenodo.org/record/8158914/files/participants.tsv

Found on: Google Scholar 
Platform: Used open dataset LEMON (Max Planck Institute Leipzig Mind-Brain-Body Dataset), MRI data, and gamma SFC matrices. Used pyClusterROI package, but platform never specified.  

SUMMARY
Purpose: Examining the multi-scale relations and connections between human brain structure, human brain function, and the associated neurogenetics. The hypothesis is that underlying neurogenetics could help in better understanding the neurological structure and function components, as well as possible connections between structural connectivity and functional modules. Certain structural connectivities do not always correspond or give rise to the associated functional modules, and this report proposes that the underlying molecular dynamics, including neurogenetics and particular transcriptomes and proteomes, somehow influence such relationships between neuronal structure and function. 
Key Problem: One of the main issues is the lack of public repositories that integrate such data (structural and functional networks of the brain, along with the associated transcriptome profiles). In addition, many brain data repositories only consider two of three variables. It therefore uses gamma parameterized modules structural-functional and the associated neurogenetic data and code (transcriptomes and connectomes) as a sort of underlying factor and correspondence. 
Contribution: gives important insight into the relations between brain structure, function, and genetics (neurogenetics), could give insight into different types of brain disorders and pathologies, as well as the brain in general (structural and functional connectivity matrices at different resolutions, with associated neurogenetic and transcriptome profiles, especially with brain pathologies). 

RELEVANCE
Theme: Combines known data about structural and functional neuron and brain correlations with the neurogenetic and neurotranscriptome profiles to generate a comprehensive view of the brain, its different regions, and the underlying molecular and biological mechanisms.  

Lab Report #2— Benchmarking drug–drug interaction prediction methods: a perspective of distribution changes
Biologist: Leeva Selioutski 
Date: 10.29.25

GitHub Code: https://github.com/LARS-research/DDI-Bench 
Found on: Google Scholar 
Platform:SUMMARY
Purpose: To create a robust benchmarking framework (DDI-Ben) that evaluates emerging drug–drug interaction prediction methods under realistic distribution changes, rather than relying on oversimplified i.i.d. splits.
Key Problem: Existing DDI prediction evaluations assume that known and new drugs follow the same distribution. This neglects real-world distribution changes (e.g., chemical novelty, approval timelines), leading to unreliable performance assessments of computational methods.
RELEVANCE
Theme:Introduces a distribution change simulation framework that models differences between known and new drug sets. 

Lab Report #3–Environmental DNA metabarcoding of lake fish communities reflects long-term data from established survey methods
Biologist: Leeva Selioutski 
Date: 10.29.25

GitHub Code:https://github.com/HullUni-bioinformatics/Haenfling_et_al_2016   
Found on: Google Scholar 
Platform: 

SUMMARY
Purpose: The study aims to investigate how genomic variation and population structure shape adaptive processes in natural populations, using large-scale sequencing approaches. It focuses on integrating ecological and evolutionary perspectives to better understand genetic diversity in the wild.
Key Problem: Traditional population genetics often relies on limited markers or small sample sizes, which restricts the ability to detect fine-scale adaptive variation. With the rise of next-generation sequencing, researchers face challenges in analyzing massive datasets and linking them to ecological context.
Contribution: Demonstrates the use of genome-wide sequencing to uncover adaptive genetic variation in natural populations.
RELEVANCE
Theme: integration of ecological context with genomic data

Lab Report #4—VAPiD, viral annotation pipeline and identification
Biologist: Leeva Selioutski 
Date: 10.29.25

GitHub Code: https://github.com/rcs333/VAPiD 
Found on: Google Scholar 
Platform: Python, Windows, Linux, MacOS

SUMMARY
Purpose: Enables easy submission of viral genomes into NCBI GenBank, which is required for publication and data availability; allows input of viruses of different genome types, such as DNA, RNA, retroviruses, and the like. Can handle individual or batch submissions of different types of viral genomes. In order to accept submitted viral genomic data, NCBI GenBank requires 1) viral sequence complete with at least one protein annotation, 2) author/depositor metadata, and 3) viral sequence metadata, such as strain, collection date, collection location, and coverage.
Key Problem: GenBank currently has automatic prokaryotic and eukaryotic genome annotation pipelines but has no viral annotation pipeline beyond influenza virus (all are DNA-based genomes). Does not include RNA-based genomes seen in quite a few viruses. Complex viral life cycles involving RNA editing, ribosomal slippage, and overlapping reading frames create certain annotation issues, along with non-standard nomenclature for viral gene products. 
Contribution: A portable and lightweight command-line tool for annotation and GenBank deposition of viral genomes, supports annotation of nearly all unsegmented viral genomes, validated for all sorts of viruses (DNA, RNA, retroviruses, etc.). Any sort of infectious disease, especially and including viruses, have the potential to spread and become epidemic. Viral genomes are made accessible through a publicly searchable database. Focus on the epidemiological or scientific insight gained from sequencing rather than rote protocols for data deposition. Provides an automatic viral genome annotation pipeline and a universal annotator regarding all virus types. 

RELEVANCE
Theme: “A portable, lightweight, user-friendly, internet-enabled, open-source, command-line genome annotation and submission package to facilitate virus genome submissions to NCBI GenBank.” “A lightweight and user-friendly command-line tool that takes FASTA files of complete or near complete viral genomes as input, automatically annotates them, and outputs the required files for GenBank submission over email.”