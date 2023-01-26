# Analysis using parallel calculations

More information about this project is in "Projekt Zaliczeniowy PDF.pdf" (only in Polish).

We received 4 files in .vcf format of Genetic data of healthy and diseased Holstein-Friesian cows. The files had more than 14.3 million records for diseased individuals and more than 13.8 mln for healthy individuals.\
The aim was to find SNP-type mutations that may have a biological basis for the development of the disease and to determine their relationship with selected parameters for each chromosome.

In this project were used libraries from Python such as Pandas, os modules, Python multiprocessing, NumPy, SciPy, and Seaborn. From R dplyr, microbenchmark, and parallel. SNPs were detected with the use of the chi2 contingency test with Yamates correction. Additionally, we examined the Pearson correlation between our results and the length of the chromosome.

Due to the enormous data, we used parallelization in Python (multiprocessing.Pool()) and R (makeCluster and clusterApply). And in a result, we discovered that project in R appeared to be faster than in Python.

![](https://github.com/Michello077/parallel-computing-analysis/blob/444bcd5a7b9fb5ec245967f7e3a80d7a09d579a6/results/PC001.png)

![](https://github.com/Michello077/parallel-computing-analysis/blob/444bcd5a7b9fb5ec245967f7e3a80d7a09d579a6/results/PC002.png)

![](https://github.com/Michello077/parallel-computing-analysis/blob/444bcd5a7b9fb5ec245967f7e3a80d7a09d579a6/results/PC003.png)

![](https://github.com/Michello077/parallel-computing-analysis/blob/444bcd5a7b9fb5ec245967f7e3a80d7a09d579a6/results/PC004.png)
