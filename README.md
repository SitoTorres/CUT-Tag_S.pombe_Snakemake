# CUT-Tag_S.pombe_Snakemake

Snakemake-based pipeline for processing of S. pombe CUT&amp;Tag data

Requires cutadapt, bowtie2, samtools (view, sort, index), deepTools (bamCoverage) and bedtools (genomecov) to be in your $PATH (or modifiy Snakefile to indicate full path to tool)

To run the pipeline:

snakemake --snakefile STG_Snakefile_CT_Sp_2024 /working/dir/{sample1,sample2,sampleX}.bw

or

snakemake --snakefile STG_Snakefile_CT_Sp_2024 /working/dir/{sample1,sample2,sampleX}_fragments.bedgraph

# input fastq (.fq.gz) file names should follow the pattern:

sample1_R1.fq.gz
sample1_R2.fq.gz

sample2_R1.fq.gz
sample2_R2.fq.gz

sampleX_R1.fq.gz
sampleX_R2.fq.gz

# Please see full Snakemake documentation at: https://snakemake.readthedocs.io/en/stable/
