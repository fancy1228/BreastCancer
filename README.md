# BreastCancer
Genetic analyses for Ashkenazi Jewish (AJ)

## Subjects
### 639 AJ breast cancer cases
phenotypes are stored at /share/data/BreastCancer/

the cases did not have BRCA1/2 mutations

265 cases are index probands

### 300 AJ controls from PCGC
biocluster: /share/shannon/xz2680/Projects/CHD/final

batch | # of samples
------------- | --------------
WES_NimbleGenV2 | 98
WES_MedExome | 112
WES_PCGC11 | 49
WES_PCGC10 | 21
WES_Goldmuntz | 8
WES_PHNv2xGEN | 5
WES_PCGC9 | 5
WES_CUMCPGM | 2

### 477 AJ controls from SPARK
biocluster: /home/xz2680/Terra/Share/SPARK/GATK4+GLnexus-UnaffFounders_PAH_Cardiomyopathy/

biocluster: /home/xz2680/Terra/Share/SPARK/JG/SPARK30K_20190729.ped

### AJ ancestry identification
shannon: /home/xf2193/Script/PCA (Xueya's pipeline)

Step 1: separate European individuals from non-European individuals

Step 2: distinguish Jewish and European individuals using AJ breast cancer cases as reference

## Sequence
AJ breast cancer cases are sequenced by Regeneron, maybe xGen

PCGC are sequenced in multiple batches using different capture kit

SPARK library was prepared using xGen regions

Jake combined lifted hg19 to hg38 and combined all cases and controls using xGen

case bams: /share/descartes/jake.proc/hg38.reproc/aj.breast.cancer/data/proc/crams

all gvcf: /share/descartes/jake.proc/hg38.reproc/aj.breast.cancer/rsrc/sample.map

combined vcf: /share/descartes/jake.proc/hg38.reproc/aj.breast.cancer/data/proc/chr.vcfs

xGen capture kit: /share/data/resources/hg38/CaptureKits/xgen_plus_spikein.b38.bed

### Processing pipeline
/share/terra/xf2193/BreastCancer/SPARK/script/batch.sh

### Quality control - GATK
deepvariants (*notused*) pipeline at shannon: /home/xf2193/Script/Pipeline

QCed data was stored: /share/terra/xf2193/BreastCancer/SPARK/QC
