##**Aggression_project**

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

| Brain Variable | r | r² | p | p (FDR) | Significant |
|---|---|---|---|---|---|
| Amygdala Vol (norm) | 0.016 | <0.001 | 0.599 | 0.652 | No |
| mOFC Gray Vol (norm) | 0.014 | <0.001 | 0.648 | 0.652 | No |
| rACC Gray Vol (norm) | 0.014 | <0.001 | 0.652 | 0.652 | No |
| mOFC Thickness | 0.047 | 0.002 | 0.122 | 0.490 | No |

**Overall, no robust associations were found between structural brain measures and self-reported anger/hostility traits in this sample. Effect sizes were uniformly negligible (r² < 0.5%), suggesting that, at least for these regions and this measure-set, structural variation does not meaningfully explain individual differences in trait anger or hostility.** The composite analysis (combining four conceptually related anger/hostility items to reduce the multiple-comparisons burden) is exploratory and follow-up to the primary screen, not an independent confirmatory test.

**Dataset**

Human Connectome Project Young Adult (HCP-YA) dataset. Data access requires a data use agreement via ConnectomeDB: https://db.humanconnectome.org

Raw data files (unrestricted_hcp_freesurfer.csv, HCP_YA_subjects_*.csv) are not included in this repository due to data use agreement restrictions. Download from ConnectomeDB and place in your working directory before running.

**Repository Contents**


Project_aggression.ipynb — full analysis notebook (data cleaning, normalisation, outlier handling, z-scoring, correlation analyses, FDR correction, composite construction)


**How to Run**


Obtain access to and download the required HCP-YA FreeSurfer and behavioural CSV files from ConnectomeDB
Place the CSV files in the same directory as the notebook (or update the file paths in the data-loading cell)
Run all cells in Project_aggression.ipynb in order


**Dependencies**

Python packages: pandas, numpy, matplotlib, seaborn, scipy, statsmodels

**References**

Anderson, C. A., & Bushman, B. J. (2002). Human aggression. Annual Review of Psychology, 53, 27–51. https://doi.org/10.1146/annurev.psych.53.100901.135231

Heilbron, N., & Prinstein, M. J. (2008). A review and reconceptualization of social aggression: Adaptive and maladaptive correlates. Clinical Child and Family Psychology Review, 11(4), 176–217. https://doi.org/10.1007/s10567-008-0037-9

Jones, S. E., Miller, J. D., & Lynam, D. R. (2011). Personality, antisocial behavior, and aggression: A meta-analytic review. Journal of Criminal Justice, 39(4), 329–337. https://doi.org/10.1016/j.jcrimjus.2011.03.004

Krämer, U. M., Jansma, H., Tempelmann, C., & Münte, T. F. (2011). Executive control in trait aggression: An fMRI study of inhibitory control using the Flanker task. Social Cognitive and Affective Neuroscience, 6(2), 180–188. https://doi.org/10.1093/scan/nsq072

Mesurado, B., Vidal, E. M., & Mestre, A. L. (2018). Negative emotions and behaviour: The role of regulatory emotional self-efficacy. Journal of Adolescence (London, England.), 64, 62–71. https://doi.org/10.1016/j.adolescence.2018.01.007

Pawliczek, C. M., Derntl, B., Kellermann, T., Kohn, N., Gur, R. C., & Habel, U. (2013). Inhibitory control and trait aggression: Neural and behavioral correlates during an emotional go/no-go task. Social Cognitive and Affective Neuroscience, 8(6), 728–735. https://doi.org/10.1093/scan/nss065

Roberton, T., Daffern, M., & Bucks, R. S. (2012). Emotion regulation and aggression. Aggression and Violent Behavior, 17(1), 72–82. https://doi.org/10.1016/j.avb.2011.09.006

Rosell, D. R., & Siever, L. J. (2015). The neurobiology of aggression and violence. CNS Spectrums, 20(3), 254–279. https://doi.org/10.1017/S109285291500019X

Siever, L. J. (2008). Neurobiology of aggression and violence. The American Journal of Psychiatry, 165(4), 429–442. https://doi.org/10.1176/appi.ajp.2008.07111774

Smith, K., Jones, A., Daly, N., Widdrington, H., Garofalo, C., & Gillespie, S. M. (2026). Emotion regulation and aggression: A systematic review and meta‐analysis. Aggressive Behavior, 52(1), e70055-n/a. https://doi.org/10.1002/ab.70055 


