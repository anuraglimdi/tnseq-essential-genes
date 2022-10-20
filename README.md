# Predicting essential genes from TnSeq data

Transposon sequencing (TnSeq) is an great approach for identifying essentiality of genes/genomic features. It involves genome-wide transposon insertion mutagenesis and high throughput sequencing based fitness assays. A lot of the downstream analysis of essentiality and fitness effects involves drawing an arbitrary cutoff for calling a gene as essential or not, typically based on prior knowledge of the biological system. 

In this project, I apply machine learning classification algorithms to predict gene essentiality in a transposon library collection in E. coli (published [here](https://www.biorxiv.org/content/10.1101/2022.05.17.492023), using the \textit{E. coli} K-12 Keio knockout collection and TraDIS as a ground truth. 

Goals of the project:
- Compare performance of different classification approaches, relative to a naive arbitrary cutoff, and examine how/why they make differing predictions
- Potentially identify non-obvious combination of TnSeq data features which underlie whether a gene is essential or not
- Develop an approach for gene essentiality classification that can account for variation in sequencing depth and other experimental parameters
- As a final validation of the approach, predict the essential genes in \textit{Acinetobacter balyayi}, which has both TnSeq and single-gene deletion data
