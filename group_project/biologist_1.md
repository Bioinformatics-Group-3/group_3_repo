**Lab Report 1**—[Building and analyzing machine learning-based warfarin dose prediction models using scikit-learn](https://doi.org/10.12793/tcp.2022.30.e22)  
**Biologist**: Sophia Fang  
**Date**: 10.22.25

**GitHub Code**: [Warfarin Prediction](https://github.com/mahlernim/warfarin_prediction_kscpt_tutorial)  
**Found on**: Google Scholar → Pharmacotherapy (PubMed Central)

**Summary**  
The Ahn paper demonstrates how to build machine learning-based warfarin dose prediction models using patient pharmacogenomic and clinical data. Warfarin is a commonly used anticoagulant with high inter-individual variability and a narrow therapeutic window, making personalized dosing critical for patient safety. The authors train three models (multiple linear regression, neural network, and random forest) on the International Warfarin Pharmacogenetics Consortium dataset, which includes patient demographics, genetic variants in CYP2C9 and VKORC1 genes, and clinical factors. The tutorial walks through the entire workflow using Python’s scikit-learn library, including data preprocessing, model training with hyperparameter tuning, performance evaluation, and interpretation through permutation feature importance and partial dependence plots.

**Relevance**  
This paper aligns perfectly with our “Pharmacogenomics & Personalized Pharmacotherapy” theme, as it demonstrates how genetic mutations in drug-metabolizing enzymes directly inform clinical treatment decisions. The CYP2C9 and VKORC1 genetic variants influence how individual patients metabolize warfarin, resulting in varying optimal doses across the population. By integrating genomic data with machine learning approaches, the paper demonstrates a practical application of translating genome-level information into personalized pharmacotherapy, which represents the core goal of precision medicine: tailoring drug treatment to individual patient characteristics to maximize efficacy while minimizing adverse effects.
 
---

**Lab Report 2**—[GenMap: ultra-fast computation of genome mappability](https://doi.org/10.1093/bioinformatics/btaa222)  
**Biologist**: Sophia Fang  
**Date**: 10.22.25

**GitHub Code**: [GenMap](https://github.com/cpockrandt/genmap)  
**Found on**: Google Scholar → Bioinformatics (Oxford University Press)

**Summary**  
GenMap is a computational tool designed to rapidly calculate genome mappability, which measures the uniqueness or repetitiveness of genomic regions—a critical factor for accurately aligning short DNA sequences (reads) to reference genomes in sequencing analyses and for designing CRISPR guide RNAs. Prior methods for computing mappability were computationally slow and often relied on heuristics that produced only approximate results, making accurate computations prohibitively expensive for large genomes. GenMap addresses these limitations by introducing an exact yet ultra-fast algorithm that efficiently computes (k, e)-mappability, which quantifies the frequency at which a sequence of length k appears in the genome when allowing up to e mismatches. This advancement enables researchers to perform precise mappability calculations on large eukaryotic genomes in reasonable time frames, opening new possibilities for genome analysis and experimental design.

**Relevance**  
GenMap’s relevance to pharmacogenomics lies in its ability to identify unique genomic regions that can be reliably sequenced and analyzed in individual patients. In personalized medicine, accurately detecting genetic variants—such as SNPs in drug-metabolizing enzymes (CYP450 genes), drug transporters, or therapeutic targets—is essential for tailoring treatment decisions. GenMap’s mappability calculations help identify which genomic regions can be confidently analyzed versus those that are too repetitive to yield reliable variant calls, directly improving the accuracy of pharmacogenomic testing. Additionally, its capability to distinguish marker sequences across similar genomes could be applied to identifying patient-specific genomic signatures that predict drug response or adverse reactions. By enabling faster and more accurate genome analysis, GenMap supports the foundational bioinformatics infrastructure necessary for implementing precision pharmacotherapy, where treatment strategies are optimized based on each patient’s unique genetic profile.

---

**Lab Report 3**—[GenomeQC: a quality assessment tool for genome assemblies and gene structure annotations](https://doi.org/10.1186/s12864-020-6568-2)  
**Biologist**: Sophia  
**Date**: 10.22.25

**GitHub Code**: [GenomeQC](https://github.com/HuffordLab/GenomeQC)  
**Found on**: Google Scholar

**Summary**  
GenomeQC is a comprehensive web-based tool designed to evaluate the quality of genome assemblies and gene structure annotations through standardized, automated metrics. As the number of genome assemblies has grown exponentially with declining sequencing costs, researchers need reliable methods to compare the completeness and accuracy of assemblies across different species and assembly types. GenomeQC addresses this need by integrating multiple quality assessment metrics into a user-friendly interface, including standard contiguity measures (N50/L50, NG(X) plots), gene space completeness (BUSCO scores), repeat space completeness (LTR Assembly Index), and vector contamination screening. The tool enables researchers to benchmark their assemblies against gold-standard reference genomes, providing both a web application for small-to-medium genomes and a Docker container for larger genomes. This makes comprehensive genome quality assessment accessible without requiring extensive computational resources or software installation expertise.

**Relevance**  
GenomeQC is relevant to pharmacogenomics because high-quality genome assemblies are essential for accurately identifying and characterizing pharmacogenes—the genes that encode drug-metabolizing enzymes (CYP450s), transporters, and therapeutic targets, which determine individual drug responses. The tool’s comprehensive quality metrics ensure that genome assemblies used for pharmacogenomic studies are sufficiently complete in both gene-rich and repetitive regions, which is critical since some pharmacogenes reside in complex genomic contexts. By enabling systematic assessment of genome quality across diverse populations, GenomeQC supports the development of more comprehensive pharmacogenomic databases that account for global genetic diversity, ultimately improving the accuracy of genotype-guided prescribing decisions in precision medicine.

---

**Lab Report 4**—[Interplay between chromosomal alterations and gene mutations shapes the evolutionary trajectory of clonal hematopoiesis](https://doi.org/10.1038/s41467-020-20565-7)  
**Biologist**: Sophia Fang  
**Date**: 11.19.25

**GitHub Code**: [Papaemmelab](https://github.com/papaemmelab/Gao_NC_CH/tree/main)  
**Found on**: Google Scholar

**Summary**  
This study investigates clonal hematopoiesis (CH)—the age-related accumulation of somatic mutations in blood cells—by jointly analyzing both gene mutations and mosaic chromosomal alterations (mCAs) in 32,442 patients with cancer. While previous CH studies have typically examined gene mutations or chromosomal alterations separately due to technical limitations, this research leveraged deep sequencing data from the MSK-IMPACT panel to simultaneously characterize both mutation types. The analysis revealed that 23% of chromosomal alterations occur in combination with specific gene mutations, forming composite genotypes that resemble known genetic interactions in leukemia. These patterns suggest that selective pressures driving leukemia development are already operating early in clonal evolution. The study identified recurrent “double-hit” events where chromosomal alterations target pre-existing mutations (in cis) and cooperative interactions between mutations on different chromosomes (in trans). Patients with these composite genotypes showed significantly elevated risk of leukemia progression (14.6% 3-year cumulative incidence), with mCAs emerging as an independent risk factor for leukemia development.

**Relevance**  
This study is relevant to pharmacogenomics through its implications for personalized cancer surveillance and treatment strategies in patients at risk of therapy-related leukemias. Understanding the mutational landscape of clonal hematopoiesis helps identify cancer patients at elevated risk of developing secondary blood cancers, which is critical for treatment planning and monitoring. The finding that mosaic chromosomal alterations are independent predictors of leukemia risk provides a framework for risk stratification that could guide decisions about therapy intensity, selection of less leukemogenic treatment regimens, and surveillance frequency. By enabling the early detection of high-risk clonal populations through routine tumor sequencing, this work supports precision medicine approaches that tailor cancer therapy based on individual genomic profiles, thereby minimizing the risk of secondary malignancies while optimizing primary treatment outcomes.

---

**Lab Report 5**—[OPUS-Fold3: a gradient-based protein all-atom folding and docking framework on TensorFlow | Briefings in Bioinformatics | Oxford Academic](https://academic.oup.com/bib/article/24/6/bbad365/7313454)  
**Biologist**: Sophia Fang  
**Date**: 11.19.25

**GitHub Code**: [OPUS-Fold3](https://github.com/OPUS-MaLab/opus_fold3)   
**Found on**: Google Scholar

**Summary**  
OPUS-Fold3 is a gradient-based, all-atom protein folding and docking framework built on TensorFlow that generates 3D protein structures based on specified constraints. Traditional protein folding frameworks like pyRosetta and CNS are powerful but difficult to integrate with modern deep learning approaches, creating a barrier between computational biology and AI communities. OPUS-Fold3 addresses this gap by implementing a flexible, Python-based framework that can simultaneously fold protein backbones and side chains while incorporating multiple constraint types—including distance/orientation distributions, experimental cryo-EM density maps, physicochemical potentials, and predictions from structure prediction methods. The framework demonstrates performance comparable to pyRosetta in backbone folding, significantly better performance in side-chain modeling, and the ability to improve correlations between atomic structures and experimental cryo-EM density maps, making it valuable for protein structure refinement, design, and experimental structure determination.

**Relevance**  
OPUS-Fold3 is relevant to pharmacogenomics through its applications in understanding drug-protein interactions at the molecular level. The framework’s ability to accurately model protein structures—including all-atom refinement and protein-protein docking—is essential for structure-based drug design targeting pharmacologically important proteins such as drug receptors, transporters, and metabolizing enzymes. By enabling researchers to refine protein structures using experimental data combined with computational predictions, OPUS-Fold3 facilitates the development of accurate structural models of pharmacogenes and their variants. This is particularly valuable for understanding how genetic variants affect protein structure and function, which directly impacts drug binding, metabolism, and efficacy, ultimately contributing to more precise predictions of patient-specific drug responses in precision medicine.

---

**Lab Report 6**—[Identifying Selections Operating on HIV-1 Reverse Transcriptase via Uniform Manifold Approximation and Projection](https://doi.org/10.1145/3569192.3569195)  
**Biologist**: Sophia Fang  
**Date**: 11.19.25

**GitHub Code**: [Epistatic](https://github.com/shefaliqamar/HIV-Epistatic)  
**Found on**: arXiv

**Summary**  
This study analyzes HIV-1 reverse transcriptase (RT) sequences from the Stanford HIV Drug Resistance Database to understand how the enzyme evolves under selective pressure from antiretroviral drugs. HIV-1’s extremely high mutation rate allows it to rapidly develop resistance to antiretroviral drugs, making it challenging to achieve sustained viral suppression. The researchers employed Uniform Manifold Approximation and Projection (UMAP), a dimensionality reduction technique designed to detect non-linear dependencies in complex data, combined with density-based clustering (DBSCAN) to identify distinct groups of RT sequences. Their analysis yielded 21 distinct sequence clusters, representing phylogenetically related sequences with strong correlations to treatment regimens. The clusters revealed patterns suggesting that HIV RT’s evolution is shaped by both drug selection and epistatic interactions (where multiple mutations work together), providing insights into the higher-order mutational dependencies that facilitate viral evolution and drug resistance.

**Relevance**  
This study is relevant to pharmacogenomics by illuminating how genetic variation in viral pathogens—specifically HIV reverse transcriptase—affects drug response and treatment outcomes. Understanding the evolutionary trajectories and mutational networks of HIV RT under antiretroviral therapy is critical for personalized treatment strategies in HIV-positive patients. The identification of distinct sequence clusters associated with specific drug regimens reveals how treatment history shapes viral evolution, which directly impacts the selection of effective antiretroviral combinations for individual patients. By mapping the epistatic interactions between resistance mutations, this work helps predict which drug combinations will remain effective in a patient’s viral genotype, supporting precision medicine approaches where treatment is tailored based on individual genetic profiles to optimize therapeutic outcomes and minimize the development of resistance.
