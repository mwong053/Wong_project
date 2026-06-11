**Aggression_project**

**Brain Structure and Aggression-Related Traits in Healthy Adults: An HCP Young Adult Analysis**

**Author:** Kok Tsz Wing, Marcus Jude Wong Shyuan

**Project Overview**

This project examines whether structural brain measures previously linked to aggression and emotion regulation — amygdala volume, medial orbitofrontal cortex (mOFC) gray matter volume and thickness, and rostral anterior cingulate cortex (rACC) gray matter volume — are associated with self-reported anger, hostility, and rejection sensitivity in a large healthy adult sample.

Using data from the Human Connectome Project Young Adult (HCP-YA) dataset (N = 1105 after quality control), bilateral FreeSurfer-derived brain volumes/thickness were normalised for intracranial volume and correlated with a battery of behavioural measures (perceived stress, self-efficacy, anger affect, anger hostility, perceived hostility, perceived rejection, inhibitory control via Flanker task, and NEO-FFI Agreeableness/Conscientiousness). False discovery rate (Benjamini-Hochberg) correction was applied across all brain-behaviour pairs. A composite "aggression-related" score (mean z-score of anger affect, anger hostility, perceived hostility, and perceived rejection) was also derived and tested against each brain measure.

**Key Findings**

**Broad screen: 4 brain measures × 10 behavioural measures (40 tests, FDR-corrected)**

All correlations were weak (|r| ≤ 0.07), and none survived FDR correction (q < 0.05). The strongest uncorrected associations were:

| Brain Variable | Behavioural Variable | r | r² | p (uncorrected) |
|---|---|---|---|---|
| rACC Gray Vol (norm) | Flanker (unadjusted) | 0.067 | 0.004 | 0.028 |
| rACC Gray Vol (norm) | NEO-FFI Agreeableness | -0.066 | 0.004 | 0.029 |
| Amygdala Vol (norm) | Flanker (unadjusted) | -0.065 | 0.004 | 0.033 |
| Amygdala Vol (norm) | Flanker (age-adjusted) | -0.061 | 0.004 | 0.044 |

**Composite anger/hostility score vs. brain structure**

Brain Variablerr²pp (FDR)SignificantAmygdala Vol (norm)0.016<0.0010.5990.652NomOFC Gray Vol (norm)0.014<0.0010.6480.652NorACC Gray Vol (norm)0.014<0.0010.6520.652NomOFC Thickness0.0470.0020.1220.490No

**Overall, no robust associations were found between structural brain measures and self-reported anger/hostility traits in this sample. Effect sizes were uniformly negligible (r² < 0.5%), suggesting that, at least for these regions and this measure-set, structural variation does not meaningfully explain individual differences in trait anger or hostility.** The composite analysis (combining four conceptually related anger/hostility items to reduce the multiple-comparisons burden) is exploratory and follow-up to the primary screen, not an independent confirmatory test.

**Dataset**

Human Connectome Project Young Adult (HCP-YA) dataset (Van Essen et al., 2013). Data access requires a data use agreement via ConnectomeDB: https://db.humanconnectome.org

Raw data files (unrestricted_hcp_freesurfer.csv, HCP_YA_subjects_*.csv) are not included in this repository due to data use agreement restrictions. Download from ConnectomeDB and place in your working directory before running.

**Repository Contents**


Project_aggression.ipynb — full analysis notebook (data cleaning, normalisation, outlier handling, z-scoring, correlation analyses, FDR correction, composite construction)


**How to Run**


Obtain access to and download the required HCP-YA FreeSurfer and behavioural CSV files from ConnectomeDB
Place the CSV files in the same directory as the notebook (or update the file paths in the data-loading cell)
Run all cells in Project_aggression.ipynb in order


**Dependencies**

Python packages: pandas, numpy, matplotlib, seaborn, scipy, statsmodels
