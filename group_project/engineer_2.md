Report # 1
Github: https://github.com/compneurobilbao/bha2 
Outcome: failure
Process: I cloned the bha2 repository and followed the instructions to run the code inside the provided devcontainer and execute the main tree-building pipeline. Although the required MRI-derived datasets are publicly available on Zenodo, the project assumes substantial prior domain-specific preprocessing and exact data organization (including SC, FC, time-series, and parcellation files) without providing a validated end-to-end script or a minimal working example to verify correctness. Even with access to the data, it was not possible to confidently execute build_tree.py without reconstructing multiple preprocessing steps and implicit assumptions that are not fully specified in the repository. As a result, I was unable to reliably run the pipeline or reproduce any of the reported outputs using the code as provided.
 
