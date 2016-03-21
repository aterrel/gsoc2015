# A general purpose next-generation sequence pre-processor for QIIME 2

### Contact Info

Name: Sourav Singh
Email: ssouravsingh12@gmail.com   
Location/Timezone: India, GMT +5:30   
University: Vishwakarma Institute of Information Technology, India     
Mentor: Greg Caporaso

## Personal Background:
### Motivation for the project:

I am a pre-final year undergraduate student Bachelors in Computer Engineering from VITT Pune, India. Being a student in Computer Engineering, I have been exposed to courses like Computer Networks, Digital Signal Processing among many others. My interest for biology got me started with Bioinformatics, and this interest intensified as I started to learn more and more about Genomics. Working with software libraries like SAMTools always inspired me to try and construct one from ground zero. I was in search of a project where I could put my efforts in this direction, and I came across projects like khmer and QIIME. As I searched further I was excited to see package which had intersections with my interests and since then have tried to contribute to it.

### Programming Skills:

My journey with open source started with Click where I had added documentation for the project, my interest in Scientific Computing introduced me to various Scientific packages like SciPy.I took various courses in Genomic Data Sciences Specialization by John Hopkins to learn about Genomics as much as possible. My interest towards hardware allowed me undertake projects involving Beaglebone Black, the details of which could be found on my GitHub repo (Repo titles : [beaglebone-codes] (https://github.com/souravsingh/beaglebone-codes)). I had an opportunity to give talks at the PyCon India 2015 on nipype, a neuroimaging package and at SciPy India 2015, where I gave a workshop on BioPython. 
 
* GitHub Profile : https://github.com/souravsingh


###Contributions to the project
I have made some pull requests to the projects which are part of the biocore like micronota, scikit-bio, QIIME 1.The pull requests can be seen here-

* Pull Request for micronota: https://github.com/biocore/micronota/pull/62
* Pull Request for scikit-bio: https://github.com/biocore/scikit-bio/pull/1297
* Pull Request for QIIME: https://github.com/biocore/qiime/pull/2134
* Pull Request for QIIME: https://github.com/biocore/qiime/pull/2133

I have also opened an issue at the numfocus repository on QIIME 2: https://github.com/numfocus/gsoc/issues/113

---
### Project Synopsis : 

The aim of the project is to equip the QIIME 2 library, which is currently under development with plugins for preprocessing of FASTA/FASTQ data so that they can be used for further downstream analysis in Taxonomic detection.
Main goals of the project include:

1. Framework to add plugins for QIIME 2 like-
    * fastq-grep
    * FastQC for Quality Control of FASTQ data
    * Trimmomatic for intelligent trimming of FASTA/FASTQ data

2. Try and Add Parallelization to some of the above tasks.

3. In the course of integration of plugins, contribute back to improve their functionality and usability.


---
---
## Timeline :

Community Bonding Period :
* Have a Thorough understanding of the various softwares that need to be added to QIIME 2.

* Get a Thorough understanding of the structure of the QIIME 2.

Goal : Get an understanding of the package and the softwares that need to be added. This would play a very crucial role in setting the pace for the project. 

Week 1 - Week 3:

*Start implementation of adding barcode-primer-sequence and barcode-primer-linker-sequence as a plugin. This should be start the setup of the preprocessing plugins for QIIME 2. Add sufficient testing machinery.

Goal : Complete implementation for barcode-primer-sequence and barcode-primer-linker-sequence as a plugin for QIIME 2.

Week 4 - Week 5:

* Implementation of barcode-linker-primer-sequence-barcode, barcode and sequence as a plugin for QIIME 2. Tests for the plugins to be added in the two weeks. Start work on Ea-utils plugin.

Goal : Complete implementation of barcode-linker-primer-sequence-barcode, barcode and sequence as a plugin for QIIME 2.

Week 6 - Week 7:

* Complete the implementation related to Ea-utils as a plugin for QIIME 2. Add test cases for the same.Work on adding fastq-tools in QIIME 2

Goal : Complete implementation related to Ea-utils for QIIME 2.

Week 8 - Week 10:

* Complete the implementation related to fastq-tools including the tests.

* Start work on the parallelization and optimization of currently implemented methods.

Goal : Complete implementation of fastq-tools. Focus on efficiency and parallelization techniques.

Week 11 - Week 13:

* Focus on efficiency and complete the work related to parallelization.

Goal : Efficiency of the implemented algorithms and parallelization techniques.

Week 14:

* Work on the documentation, fixing bugs and polishing the work to be ready for Master.

---
### Post GSoC :
I would love to continue contributing to QIIME 2 :)