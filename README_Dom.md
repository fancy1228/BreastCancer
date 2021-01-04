# BreastCancer
Genetic analyses for Dominican (Dom) American

## Subjects
### 501 familial Dom breast cancer cases
phenotypes are stored at /share/data/BreastCancer/doc

the cases did not have BRCA1/2 mutations

130 cases are index probands

### 1300 Dom controls from WHICAP
biocluster: /share/descartes/jake.proc/hg38.reproc/whicap/data/proc/

old people enrolled for Alzheimer's Disease from Washington Height

noted: SPARK Hispanic are native American admixture and not matched to Dom

### Dom ancestry matching
biocluster: /share/terra/xf2193/BreastCancer/Hispanic/script/

Step 1: run_peddy.sh to identify Hispanic

Step 2: SPARK_whicap_hispanic.R to match 10x controls using nearest neighbors

## Sequence
Dom breast cancer cases are sequenced by Regeneron, maybe xGen

WHICAP are sequenced by IGM

Jake combined lift-over hg38 from hg19 and combined all cases and controls using xGen

case bams: /share/descartes/jake.proc/hispanic_breastCancer/data/proc/crams

all gvcf: /share/descartes/jake.proc/hispanic_breastCancer/data/proc/gvcfs

combined vcf: /share/descartes/jake.proc/hispanic_breastCancer/data/proc/vcfs

xGen capture kit: /share/data/resources/hg38/CaptureKits/xgen_plus_spikein.b38.bed

### Processing pipeline
/share/terra/xf2193/BreastCancer/Hispanic/script/batch.sh

### Quality control - GATK
deepvariants (*notused*) pipeline at shannon: /home/xf2193/Script/Pipeline

QCed data was stored: /share/terra/xf2193/BreastCancer/Hispanic/QC
