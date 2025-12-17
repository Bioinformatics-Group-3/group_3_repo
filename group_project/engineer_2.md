Report # 1
-Github: https://github.com/compneurobilbao/bha2 
-Outcome: failure
-Process: I cloned the bha2 repository and followed the instructions to run the code inside the provided devcontainer and execute the main tree-building pipeline. Although the required MRI-derived datasets are publicly available on Zenodo, the project assumes substantial prior domain-specific preprocessing and exact data organization (including SC, FC, time-series, and parcellation files) without providing a validated end-to-end script or a minimal working example to verify correctness. Even with access to the data, it was not possible to confidently execute build_tree.py without reconstructing multiple preprocessing steps and implicit assumptions that are not fully specified in the repository. As a result, I was unable to reliably run the pipeline or reproduce any of the reported outputs using the code as provided.
-Engineer: Rayhan Zaman

Report # 2
-Github: https://github.com/LARS-research/DDI-Bench
-Outcome: partial success
-Process:  I started by cloning the DDI‑Bench repo and setting up a conda environment with Python 3.8, then spent a bunch of time wrestling with different PyTorch, DGL, and PyG versions to make the baselines work. I eventually got the main DDI‑Bench models like MSTE and MLP running on the DrugBank dataset after reinstalling CPU‑only PyTorch a few times and fixing dependency conflicts. After that, I moved on to the EmerGNN models, which were much harder to get working and I kept switching between PyTorch 1.10 and 1.12, reinstalling torch‑scatter, torch‑sparse, and the rest of the PyG stack just to get evaluate.py to run with different GPU flags, but I did manage to get EmerGNN to execute in CPU mode. Finally, I tried to get DDI‑GPT working. At first, the BioGPT model inside the repo wouldn’t load properly because important weights were uninitialized, so I manually created a biogpt folder and downloaded the HuggingFace model. After installing transformers and sacremoses, I was finally able to run main_drugbank.py with the cluster split strategy. I never got TextDDI fully working with all dataset types, ot DDI‑GPT but the core DDI‑Bench models were the ones I successfully ran.
-Engineer: Rayhan Zaman 

Report # 3
-Github: https://github.com/HullUni-bioinformatics/Haenfling_et_al_2016   
-Outcome: failure 
-Process: I cloned the Haenfling_et_al_2016 repository and carefully reviewed the README and accompanying documentation, which describe a reproducible eDNA metabarcoding workflow based on the metaBEAT pipeline and Docker. I installed Docker locally and attempted to run the provided metaBEAT container as instructed, mounting the repository directory into the container and exploring the 12S and CytB Jupyter notebooks intended to reproduce the analyses from the paper. While the container itself could be launched successfully, I quickly encountered blocking issues related to missing raw sequencing data. The repository does not include the original Illumina FASTQ files and instead assumes that the user will manually download dozens of SRA accessions from NCBI and organize them into a very specific directory structure with exact file naming conventions. I attempted to download a subset of the required SRA datasets using the SRA Toolkit and convert them to FASTQ format, but the notebooks and metaBEAT commands depend on a complete and correctly named set of samples across multiple markers, making partial execution infeasible.
-Engineer: Rayhan Zaman 

Report # 4
-Github: https://github.com/rcs333/VAPiD
-Outcome: success/fail 
-Process: I Installed the software and its dependencies according to the provided instructions. The package could be executed using the included reference database, and the core functionality ran without runtime errors, confirming that the codebase is usable and correctly configured. However, while the tool itself works as intended, the repository does not provide a clearly defined experimental pipeline, parameter configuration, or expected quantitative outputs corresponding to the figures or results reported in the associated article. As a result, although I was able to run the software on the reference data and verify that it executes, there were no specific published results that could be directly recreated or quantitatively compared to the paper.
-Engineer: Rayhan Zaman 

