## Example of workshop content: using FASTQC

### Overview

In this section, we will download a small data file containing sequence data from yeast, and then use the `fastqc` command to assess the quality of the data.

#### Learning Objectives

By the end of this section of the course you will have learned:

 1. How to set up your directory structure for your analysis project
 2. How to download the sequencing data (in fastq format) from FigShare
 3. How to run the `fastqc` command (via the command line) and direct the output to a specific directory.

### Setting up your project directories

*Add commentary...*

```
# Create directory in which to perform analysis, and change to that directory
mkdir YeastAnalysis
cd YeastAnalysis
```

*Add commentary...*

```
# Create subdirectories to hold data and output from FASTQC
mkdir fastq
mkdir fastqc_output
```

### Downloading the data

*Add commentary...*

```
# Change to data directory, and download data from FigShare
cd fastq
wget -O yeast.fastq https://ndownloader.figshare.com/files/4790242
```

### Running `fastqc` on the command line

*Add commentary...*

```
# Run fastqc command on the file yeast.fastq and save the output in fastqc_output
fastqc -o ../fastqc_output yeast.fastq
```