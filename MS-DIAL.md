# MS-DIAL
Version: 5.1.23

![image](https://github.com/user-attachments/assets/1d58f197-bf95-4af9-8c91-4303d51ae2f3)

## Website
https://systemsomicslab.github.io/compms/msdial/main.html

## Description
For untargeted data-independent acquisition (DIA) tandem MS data, this software offers deconvolution. To facilitate quick data extraction, the data are first transformed into the Analysis Base File (ABF) format. The approach starts with a smoothing technique for peak identification, which may involve moving averages, Savitzky-Golay filters, linearly weighted smoothing averages, or binomial filters for accurate mass and retention time. The Savitzky-Golay filter is used to determine the first-order derivative (FF), second-order derivative (SF), and median amplitude (AF) in order to identify peaks. The method determines the maxima of the first and second derivatives by detecting the largest amplitude difference between neighboring peaks. When the amplitude and first-order derivative surpass AF and FF at two nearby sites, peak edges are identified. When the sign of the first derivative changes and the second derivative is less than SF, the peak tip is found. Accurate mass and retention time are used in two-dimensional peak identification, often known as "peak spotting" (MS1). Spots with the same retention duration and comparable m/z are evaluated by peak height to see if they should be merged. Detected peak tops are shown as spots. Each peak is resolved using the MS²Dec algorithm, designed to extract product spectra for all precursor peaks across MS/MS spectra. This method adapts GC-MS deconvolution principles, substituting nominal mass with accurate mass. It employs least squares optimization to isolate model peaks from chromatograms, effectively minimizing background noise and separating coeluted metabolites by evaluating reconstructed chromatograms’ peak intensities. After smoothing, baseline correction identifies local minima within user-defined segments, calculates their median, and excludes points exceeding this threshold. To qualify as model peaks, ideal slope and sharpness values are determined, requiring a slope >0.95. Metabolites are identified by referencing databases such as MassBank, LipidBlast, NIST, or custom libraries, with identification scores based on the similarity of MS/MS spectra, MS1 data, retention time (RT), and isotope patterns.Peak alignment leverages an algorithm inspired by the Joint Aligner in MZmine, with support for imputing missing values. The software was specifically tested using sequential windowed acquisition of all theoretical (SWATH) acquisition, a data-independent acquisition (DIA) method.

## Functionality
- Preprocessing

## Instrument Data Type
- MS/LC-MS/LC-MS/MS
- GC/GC-MS/GC-MS/MS

## Approach
- Untargeted chemical compounds

## Software Type
Package

## Interface
- Command line interface
- Graphical user interface

## Operating System (OS)
Windows

## Language
C#

## Dependencies
≥ .NET Famework 4.0, ≥4GB RAM, x64

## Input Formats - Open
.mzML

## Input Formats - Proprietary
Agilent .d, AB Sciex .wiff, Thermo Fisher Scientific .raw, Bruker Daltonics .d, waters .raw

## Published
2015

## Last Updated
2024

## License

## Publications
- https://www.nature.com/articles/s41587-020-0531-2 (2020)
- https://www.nature.com/articles/s41592-019-0358-2 (2019)
- https://www.nature.com/articles/nmeth.4512 (2017)
- https://pubmed.ncbi.nlm.nih.gov/25938372/ (2015)
