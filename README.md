# scRNAseq-Workshop
In this workshop we will go through the basics of single cell RNA-seq analysis (scRNA-seq).
We will start with a short introduction of single cell technologies and how they can be used to better understand disease and treatment in precision medicine.

We will then begin the practical part of the course, where a COVID-19 dataset of patients PBMCs will be provided for analysis. The goal is for the particpants to understand and run pre-written code to process and analyze the dataset using the Seurat package. The code also can be used as basis for additional analyzes.

Requirements for this workshop include:
-	Personal laptop (don’t forget the power cable)
-	R installed (follow the steps at https://www.r-project.org)
-	R studio installed (follow the steps at https://www.rstudio.com/products/rstudio/download/ free version)
-	R memory limit maxed (different for windows, mac and unix, see below)

To re-set the memory in windows please run in R:
	install.package(‘utils’)
	memory.limit(320000000000)

To re-set the memory in mac please run in the terminal:
cd ~
touch .Renviron
open .Renviron

re-write in the open window
R_MAX_VSIZE=320000000000

To re-set the memory in unix please run in R:
devtools::install_github("krlmlr/ulimit")
ulimit::memory_limit(320000000000)

Note: The limit exemplified is the limit of my personal laptop, you will have to tailor it to your own laptop.
