# mhLZ-Metagenome-Project
Codes for data cleanup 

Log on to Genome Center Server- Get username and password

ssh USERNAME@cabernet.genomecenter.ucdavis.edu
Will be prompted for password

Useful commands:


cd - moves through directories

cd .. - moves up 1 directory

ls - look at content of directory

sbatch - submits a job (script) into the queue (gets in line- use for large jobs/ for loops)

bash - runs a job from the head node (immediately runs, only use for small jobs!)

scancel - cancels a job on the queue (type job ID after scancel)

watch squeue -u : watches submited jobs (type username after -u)

nano - opens text editor for writing/editing scripts

When writing scripts inclde shebang and header usually:
#!/bin/bash
##
#SBATCH -o /share/tearlab/Maga/Stephanie/Scripts/mothur_fasta.out
#SBATCH -e /share/tearlab/Maga/Stephanie/Scripts/mothur_fasta.err
#SBATCH -n 4
#SBATCH -t 8-00:00:00
