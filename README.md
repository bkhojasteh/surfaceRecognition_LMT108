# Multimodal Multi-User Surface Recognition with the Kernel Two-Sample Test

This codebase generates the results of the journal paper **Multimodal Multi-User Surface Recognition with the Kernel Two-Sample Test**, Behnam Khojasteh, Friedrich Solowjow, Sebastian Trimpe, Katherine J. Kuchenbecker, *IEEE Transactions on Automation Science and Engineering (T-ASE)*, 2023. 

We used MATLAB R2020b for this publication. 

If you use our code, we would appreciate it if you could cite our corresponding paper:
```bibtex
@article{khojasteh2023multimodal,
  title={Multimodal Multi-User Surface Recognition with the Kernel Two-Sample Test},
  author={Khojasteh, Behnam and Solowjow, Friedrich and Trimpe, Sebastian and Kuchenbecker, Katherine J.},
  journal={IEEE Transactions on Automation Science and Engineering (T-ASE)},
  year={2023}
}
```

## File Structure
The content of the zip file "code_surfaceRecognitionLMT108_TASE2023.zip" is organized as follows:

Several MATLAB computation scripts for various conditions: 
- Main publication result: mainResult_LMT108_n400_R10_8infos_5shifts.m
- 10 vs. 1 classification setting: LMT108_n400_8infos_10vs1.m
- 1 vs. 10 ablation studies: LMT108_n400_R10_Expert_vs_Users_AblationStudies.m
- 1 vs. 1 ablation studies: LMT108_n400_R10_Expert_vs_Expert_AblationStudies.m
- HSIC results for Figure 7: HSIC_mixing_2surfaces_IRsignals.m

The MATLAB file "ClassificationEvaluation.m" evaluates the outcome of our classifier for various conditions.

The folder /supportFunctions includes additional modules that are used for the computations.

The zip file "data_results.zip" can be downloaded from https://doi.org/10.5281/zenodo.8077639 and contains the following folders:

The folder /DataLMT108 contains the processed data from LMT108 surface database (https://zeus.lmt.ei.tum.de/downloads/texture).

The folder /Results contains the saved results of the computation scripts.


## References
We test our recognition framework on a public surface dataset (LMT108), using existing implementations of the standard kernel two-sample test (MMD) and Hilbert Schmidt Independence Criterion (HSIC).

The links to the original sources are as follows:

- LMT108 surface database: https://zeus.lmt.ei.tum.de/downloads/texture
- MMD estimator from Gretton, A., K. Borgwardt, M. Rasch, B. Schoelkopf and A. Smola: A Kernel Two-Sample Test. JMLR 2012: http://www.gatsby.ucl.ac.uk/~gretton/mmd/mmd.htm
- HSIC estimator from Gretton, A., K. Fukumizu, C.-H. Teo, L. Song, B. Schoelkopf and A. Smola: A Kernel Statistical Test of Independence. NIPS 21, 2007: http://people.kyb.tuebingen.mpg.de/arthur/indep.htm


## Contact Information
If you have any questions, feel free to reach out to us:

- Behnam Khojasteh: khojasteh@is.mpg.de
- Friedrich Solowjow: friedrich.solowjow@dsme.rwth-aachen.de
- Sebastian Trimpe: trimpe@dsme.rwth-aachen.de
- Katherine J. Kuchenbecker: kjk@is.mpg.de

Disclaimer: This code is provided as-is, and while we have put effort into ensuring its quality, we cannot guarantee that it is free from bugs or errors. Please use at your own discretion.
