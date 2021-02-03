## Content creation example


### Background

In this section we are going to step through the process of creating a short piece of workshop content, where we have attendees:

 - create a directory structure for their analysis
 - download a small genomic data set
 - run a command to process this data 

Having a simple (preferably well-commented) shell script which carries out the required commands is a good starting point to build a workshop component around.

The following script provides an example:

```
!/bin/sh

# Create directory in which to perform analysis, and change to that directory
mkdir YeastAnalysis
cd YeastAnalysis

# Create subdirectories to hold data and output from FASTQC
mkdir fastq
mkdir fastqc_output

# Change to data directory, and download data from FigShare
cd fastq
wget -O yeast.fastq https://ndownloader.figshare.com/files/4790242

# Run fastqc command on the file yeast.fastq and save the output in fastqc_output
fastqc -o ../fastqc_output yeast.fastq
```

### Generating content


