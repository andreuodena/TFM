# Local input data

Place the following files in this directory before running the preprocessing
analysis:

- `260824_Counts.csv`: semicolon-delimited gene-count matrix with `gene_name`
  as the first column and one PDX model per remaining column.
- `260824_Metadata.csv`: semicolon-delimited model metadata containing at least
  `samples`, `Batch` and `Subtype_2`.

These files are intentionally excluded from version control. Both the bulk
RNA-seq preprocessing and PAM50-classification analyses use these two files.

The olaparib-cisplatin analysis additionally requires:

- `260827_Metadata_PARPi_Cisplatin.csv`: semicolon-delimited metadata containing
  `samples`, `best_response_olap`, `best_response_cisplatin`,
  `Olaparib_(PARP1-2i)_response` and
  `Cisplatin_(platin_chemo)_response`.

The paired acquired-resistance analysis additionally requires:

- `COUNTS_PARPi_Resistance_Cohort.csv`: semicolon-delimited count matrix with
  `id_gene`, `gene_name` and the 28 sample columns.
- `Metadata_PARPi_Resistance_Cohort.csv`: semicolon-delimited annotations with
  `sample_id`, `pdx_id`, `patient_id`, `olaparib_sensitivity` and
  `treatment_status`.
