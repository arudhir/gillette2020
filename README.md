# gillette2020
Cleaned transomic dataset for 99 tumor/normal adjacent tissue samples from treatment-naive lung cancer patients

Data comes from https://pubmed.ncbi.nlm.nih.gov/32649874/ and is in `data/`

* variants.csv: Contains the genes that are mutated and the broad impact (HIGH, LOW, MODERATE, MODIFIER) those mutations would have on protein function
* rna.csv: Counts in TPM. Indexed by gene symbol, columns are samples
* prot.csv: Abundance ratios. Indexed by gene symbol, columns are samples 
* phos.csv: Abundance ratios. Indexed by gene symbol and phosphosite, columns are samples
* metadata.csv: Indexed by sample. A single patient gives two samples: tumor and adjacent tissue that is normal. e.g. `C3L.00001.N` is the normal sample from patient C3L.00001, and `C3L.00001` is the tumor sample from the same patient
* clinical.xlsx: a bunch of stuff from the doctors about these patients and tumors. Indexed by patient. The `case_id` column is the patient ID I referred to earlier.
