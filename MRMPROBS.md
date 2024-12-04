# MRMPROBS (including MRMDIFF) 
Version: 3.71

## Website
https://systemsomicslab.github.io/compms/mrmprobs/main.html

## Description
An open-access RIKEN program called Multiple Reaction Monitoring-Based Probabilistic System for Widely Targeted Metabolomics (MRMPROBS) offers statistical analysis along with automatic fragment identification and annotation from MRM experiments. Peaks are first found, categorized, and smoothed. Using a Savitzky-Golay filter, the median amplitude (AF), first-order derivative (FF), and second-order derivative (SF) are calculated in order to detect peaks. The maxima of the first and second-order derivatives are determined, as well as the maximum amplitude difference between two neighboring peaks. Peaks are said to have edges when their amplitude and first-order derivative both surpass AF and FF at two nearby sites and tips when the first derivative's sign shifts and the second-order derivative falls below SF. Each metabolite peak is then given a score based on its intensity, retention time, qualifier/target (QT) ratio, shape, and coelution similarity. The posterior probability (odds ratio in multivariate logistic regression) is then used to evaluate the peaks. The QT ratio and retention time are evaluated using the Gaussian function. By comparing the peak height to the highest peak in each transition record and its rank inside a particular transition record, peak intensity is assessed. The mProphet algorithm is used to evaluate shape and coelution similarity. Peak groups are assessed using the QT ratio, in which the qualifier transitions separate the metabolite from isomeric metabolites and background noise while the target transition quantifies the metabolite. The quantification value is chosen from peak groups that have the highest likelihood. Metabolites are detected in this technique by comparing them to a reference library. By employing LOWESS (QC samples) regression with a second-degree least-squares robust tri-cubic weight function, metabolite intensities can be normalized to an internal standard. After that, statistical analysis can be carried out using the multiple t-tests and PCA options.


## Functionality
- Preprocessing data

## Instrument Data Type
- MS/GC-MS/GC-QqQ-MS
- MS/LC-MS/LC-QqQ-MS

## Software Type
Package

## Interface
Graphical user interface

## Operating System (OS)
Windows x64

## Language
C#

## Dependencies
≥ .NET Famework 4.0

## Input Formats
Reifycs .ABF, .mzML

## Input Formats - Proprietary
Agilent .d, AB Sciex .wiff, Thermo Fisher Scientific .raw, Shimadzu .LCD

## First published
2013

## Last Updated
2024

## License

## Publications
https://pubmed.ncbi.nlm.nih.gov/25688256/ (2015)
https://pubmed.ncbi.nlm.nih.gov/24753485/ (2014)
http://www.ncbi.nlm.nih.gov/pubmed/23581547 (2013)

