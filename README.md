PROJECT1
1.echo Akogwu_Ngbede_Ocholi
2.mkdir Akogwu_Ngbede_Ocholi
3.cd Akogwu_Ngbede_Ocholi biocomputing ../ 
4a. wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna
4b. curl https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
4c. wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
5. mv wildtype.fna Akogwu_Ngbede_Acholi
6. rm wildtype.gbk
7. grep 'tata' wildtype.fna
8. pwd
9. head -v wildtype.gbk
10. grep ' locus' wildtype.gbk
11. grep ' source ' wildtype.gbk
12. ls -lh | grep 'gene='
13. history
14. ls -a

PROJECT 2

1a.wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
b. bash Miniconda3-latest-Linux-x86_64.sh
c. conda --version
2. conda create -n funtools  python=3.10
3. conda activate funtools
4a.sudo apt-get update
b. sudo apt-get install figlet
5. 'figlet AKOGWU NGBEDE'
6. sudo apt-get bwa
7.sudo apt-get install blast
8.sudo apt-get install Samtools
9.sudo apt-get install bedtools
10 sudo apt-get install spades.spy
11.sudo apt-get install bcftools
12.sudo apt-get install fastp
13.sudo apt-get install multiqc
