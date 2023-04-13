# GBS - From fastq files to graph

This project has been done to make gbs analysis easier for researchers with low programming knowledge.
The data preparation has been done on Narval cluster from Compute Canada and the R analysis has been made on Windows 11 and might not work on another platform.


## Prerequisite

To fullfil the prerequisite you will need your sequencing data and phenotyping data. Here are the list of things you will need:

### Files


### Softwares
| Software | Use |
| :---: | --- |
| [Sabre][SabreREF] | Sabre is a barcode demultiplexing and trimming tool for FastQ files. |
| [Cutadapt][CutadaptREF] | Cutadapt is a tool that finds and removes adapter sequences, primers, poly-A tails and other types of unwanted sequence from your high-throughput sequencing reads. |
| [BWA][bwaREF] |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |


## Prepering linux environment
Once you've recieved your sequencing data, you will need to place them in a new empty folder. To that folder, you will add your barcode file, the reference genome fasta file and all the script files of this project. 

### Extract compressed file
This type of compressed file (.gz) can be unziped usig gunzip (gzip) function. Unsing the command prompt, go to the sequencing data file directory and write `gzip -dk file.gz` where file is replaced by your file name. This function ask `gzip` to `d`ecompress and `k`eep an orginal ziped version of your file.


## Notes GBS

##


## Nettoyage des séquences
1. Demultiplexing
   Separer les séquences selon leur code barre à l'aide du script sabre et du fichier avec les séquences de codes barres

2. Trimming
   Retirer les adapteurs des séquences à l'aide du script cutadapt et du fichier contenant les séquences des adapteurs

3. Qualité des reads
   Évaluer la qualité des reads à l'aide de FastQC?

## Étapes après nettoyage
1. FASTQ -> SAM
   Utiliser le script BWA pour alligner les séquences sur le gène de référence.

2. SAM -> BAM
   Utiliser samtools

3. BAM -> VCF
   Utiliser vcftools






[SabreREF]: https://github.com/najoshi/sabre
[CutadaptREF]: https://cutadapt.readthedocs.io/en/stable/index.html
[bwaREF]: https://bio-bwa.sourceforge.net/











pour une img
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"


block code
```
mon code
```

