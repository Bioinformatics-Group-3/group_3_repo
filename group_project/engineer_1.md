Report #1
Github: https://github.com/mahlernim/warfarin_prediction_kscpt_tutorial
Outcome: Partial success.
Process: I cloned the repo and tried to run the main Jupyter notebook (KSCPT workshop.ipynb). The notebook uses a cleaned IWPC dataset (IWPC_cleaned.csv) that’s already included, which is nice because I didn’t have to do the full data-cleaning pipeline myself. I was able to get the earlier parts working (loading the data and running the basic model training steps). But one later section broke because the code calls a scikit-learn function that doesn’t exist anymore in newer versions. Specifically, the notebook uses sklearn.inspection.plot_partial_dependence to make partial dependence plots. That function was deprecated and then removed in newer scikit-learn releases, so my run failed at that point with an error about the function being missing. To fix it, I would either need to install an older scikit-learn version that still has that function (the paper reports using scikit-learn 1.0.1), or update the code to use the modern replacement (PartialDependenceDisplay.from_estimator). Because I couldn’t complete the partial dependence plot section as written, I wasn’t able to fully run the whole tutorial end-to-end in my current environment.
Engineer: Haider Gilani 


Report #2
Github: https://github.com/cpockrandt/genmap
Outcome: Partial success.
Process: I cloned the genmap repo and followed the README. GenMap is a command-line C++ tool that computes genome “mappability” (how unique each k-mer is) while allowing up to e mismatches, and it can export results in formats like WIG and BED/bedGraph. I installed it through Bioconda to avoid dealing with CMake/submodules and compiler issues. After installing, I could run the basic workflow: build an index from a FASTA file and then compute mappability, which writes text + wig + bedGraph outputs. Where I got stuck was reproducing the paper-level results (runtime/benchmark comparisons and the exact experimental setups). The repo is “not actively maintained,” and while it explains how to run the tool, it doesn’t provide a clean, one-command benchmark pipeline with pinned genome versions and settings that would let me recreate the paper’s tables/claims in a straightforward way. So the tool itself ran for me on test inputs, but I couldn’t fully replicate the paper’s reported benchmarking results.
Engineer: Haider Gilani 

