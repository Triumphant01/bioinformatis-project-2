#PROJECT FOR STAGE 0 HACKBIO BIOINFORMATICS INTERNSHIP 
1. # I will print my name 
$echo Akogwu 
2.# I will create a folder titled Akogwu 
$mkdir Akogwu 
3. # I will create another directory titled 'biocomputing' and change to this directory 
$mkdir biocomputing && cd biocomputing 
4.# I will download 3 files from hackbio website using the link.
$wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna && wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk && wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
5.#i will move ' .fna' file to the folder titled Akogwu 
$mv wildtype.fna Akogwu 
6.#i will delete the duplicate 'gbk' file.
$rm wildtype.gbk
7.# I want to confirm if the '.fna' file is mutant or wildtype('tatatata' VS 'tata')
$grep 'tatatata' ../Akogwu/ wildtype.fna && grep 'tata' ../Akogwu/wild type
8.# the file is mutant so I will print all matching lines into a new file 
$grep 'tatatata' ../Akogwu/wildtype.fna>mutant lines.txt
9.#i will count the number of lines (excluding the header) in the '.gbk' file 
$wc -l wild type.gbk
10.#i will print the sequence length of the '.gbk' file (use the 'LOCUS' tag in the first line)
$awk '/^LOCUS/ {print $3}' wildtype.gbk
11.#i will print the source of the '.gbk' file.(Use the 'Use the 'SOURCE' tag in the first line)
$$awk '/^SOURCE/ {print $3}' wildtype.gbk
12.#I will list all gene names of the '.gbk' file.hint{'grep'/gene='}
$grep 'gene=wildtype.gbk | sort -u
13.#i will clear my terminal space and print all commands used today 
$exit && history 
14.#i will list the file in the folders
$ls && ls ../Akogwu

#PROJECT 2. INSTALLING BIOINFORMATICS SOFTWARE ON THE TERMINAL 
1.#I will activate my conda environment 
$wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
2.# I will create a conda environment named ' funtools '
$conda create -n funtools 
3.#i will activate funtools 
$conda activate funtools
4.#i will install figlet 
$sudo apt-get install figlet 
5.#I will write my name and run it on figlet 
$figlet Akogwu 
6.#i will install BWA
$sudo apt-get install BWA
7.#i will install blast
$sudo apt-get install ncbi-blast+
8.#i will install samtools
$sudo apt-get install samtools 
9.#i will install bedtools
$sudo apt-get install bedtools 
10. # I will install spades.py
$spades.py
11.#i will install bcftools
$sudo apt-get install bcftools 
12.#i will install fastp
$sudo apt-get install fastp 
13.#i will install multiqc
$pip install multiqc 
