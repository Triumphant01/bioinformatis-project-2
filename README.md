PROJECT FOR STAGE 0 HACKBIO BIOINFORMATICS INTERNSHIP 
 # I will print my name 
echo Akogwu 
# I will create a folder titled Akogwu 
mkdir Akogwu 
# I will create another directory titled 'biocomputing' and change to this directory 
mkdir biocomputing && cd biocomputing 
# I will download 3 files from hackbio website using the link.
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna && wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
#i will move ' .fna' file to the folder titled Akogwu 
mv wildtype.fna Akogwu 
#i will delete the duplicate 'gbk' file.
rm wildtype.gbk.1 Akogwu 
# I want to confirm if the '.fna' file is mutant or wildtype('tatatata' VS 'tata')
grep 'tatatata' ../Akogwu/ wildtype.fna && grep 'tata' ../Akogwu/wildtype.fna
# the file is mutant so I will print all matching lines into a new file 
cat mutant_lines.fna
#i will count the number of lines (excluding the header) in the '.gbk' file 
tail -n +2 wild type.gbk | wc -l
#i will print the sequence length of the '.gbk' file (use the 'LOCUS' tag in the first line)
awk '/^LOCUS/ {print $3}' wildtype.gbk
#i will print the source of the '.gbk' file.(Use the 'Use the 'SOURCE' tag in the first line)
awk '^SOURCE' wildtype.gbk | head -1
#I will list all gene names of the '.gbk' file.hint{'grep'/gene='}
grep 'gene=wildtype.gbk | sort -u
#i will clear my terminal space and print all commands used today 
exit && history 
#i will list the file in the folders
ls && ls ../Akogwu

#PROJECT 2. INSTALLING BIOINFORMATICS SOFTWARE ON THE TERMINAL 
#I will activate my conda environment 
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
# I will create a conda environment named ' funtools '
conda create -n funtools 
#i will activate funtools 
conda activate funtools 
#i will install figlet 
sudo apt-get install figlet 
#I will write my name and run it on figlet 
figlet Akogwu 
#i will install BWA
conda install -c bioconda BWA
#i will install blast
conda install -c bioconda ncbi-blast+
#i will install samtools
conda install -c bioconda samtools 
#i will install bedtools
conda install -c bioconda bedtools 
 # I will install spades.py
conda install -c bioconda spades.py
#i will install bcftools
conda install -c bioconda bcftools 
#i will install fastp
conda install -c bioconda fastp 
#i will install multiqc
pip install multiqc 



my GitHub links.
https://github.com/Triumphant01/bioinformatis-project-2.git

My Group
https://www.linkedin.com/posts/opemidimejiosatoyinbo_teamabrlovelace-hackbio-biocoding-activity-7367517382656847874-Jffr?utm_source=share&utm_medium=member_android&rcm=ACoAADmaLP4BTSii6SvEVOmE3W9ZM_2MQIBcBPg
