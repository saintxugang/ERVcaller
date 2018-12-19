# ERVcaller
ERVcaller is a tool designed to accurately detect and genotype non-reference unfixed endogenous retroviruses (ERVs) and other transposon elements (TEs) in the human genome using next-generation sequencing (NGS) data. We evaluated the tool using both simulated and benchmark whole-genome sequencing (WGS) datasets. ERVcaller is capable of accurately detecting various TE insertions of any length, particularly ERVs. It can be applied to both paired-end and single-end WGS, WES, or targeted DNA sequencing data. It supports the use of FASTQ or BAM files(s) generated by different aligners (only BWA, Bowtie were tested). In addition, ERVcaller is capable of detecting insertion breakpoints at single-nucleotide resolution. It allows for the use of either consensus TE sequences or a TE library containing abundant TE sequences as the reference, such as the entire RepBase database. Thus, ERVcaller can be used to detect insertions from highly mutated or novel TE sequences. It is easy to install and use with the command line.

Complementary to ERVcaller, other bioinformatics tools designed to detect large deletions may be used to detect TEs that are present in the human reference genome but not in testing samples.

2 Installation
2.1 Extract the latest ERVcaller installer
$ tar vxzf ERVcaller_v.1.3.tar.gz

2.2 Installing dependent software
Users need to successfully install the following software separately and make them available in the default search path (such as by using the Linux command “export” or adding them to your .bashrc).

BWA-0.7.10: http://bio-bwa.sourceforge.net/bwa.shtml
Bowtie2: http://bowtie-bio.sourceforge.net/bowtie2/manual.shtml
