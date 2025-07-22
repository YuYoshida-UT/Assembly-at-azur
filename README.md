# Assembly-at-azur
# fastpでDNBSEQショットガンシーケンスを処理
conda create -n assembly -y
conda activate assembly
mamba install -c bioconda -y fastp
fastp --in1 DNBSEQ_M042_Read1.fq.gz --in2 DNBSEQ_M042_Read2.fq.gz --out1 QFDNBSEQ_M042_Read1.fq.gz --out2 QFDNBSEQ_M042_Read2.fq.gz --thread 16
fastp --in1 DNBSEQ_M293_Read1.fq.gz --in2 DNBSEQ_M293_Read2.fq.gz --out1 QFDNBSEQ_M293_Read1.fq.gz --out2 QFDNBSEQ_M293_Read2.fq.gz --thread 16
#ctrl+Z & bg 
