# The task was to implement different softwares on multiple datasets

Before implementing the softwares, some tasks were carried out. They include:

1. Counting of the number of sequences in a file, DNA.fa. To do this, i used the command below

    tail -n +2 DNA.fa | tr -d '\n' | wc -c

2. Afterwards, the total number of A, T, G and C in the file was determined using

   grep -Eo 'A|T|G|C' DNA.fa | sort | uniq -c | awk '{print $2": "$1}'

## Then, the softwares to be used were downloaded. The softwares are:

1. fastp
2. fastqc
3. bwa
4. samtools

This was done by using the following command

    sudo apt-get install software

The datasets to be worked on were downloaded using 'wget' which was downloaded using

    sudo apt-get install wget

The following command was used to download the datasets

    wget datasetlink

