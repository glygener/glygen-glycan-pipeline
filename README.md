# README

This repository contains file tracking information for the glycan data pipeline between GW and Georgetown. The tracking file "files4nathan.csv" contains the following information:
|Field name|Description|
|------|------|
|File name|Name of file|
|Path|Path from downloads folder|
|Source|Data source/provider|
|GlyGen Datasets|Dataset ID for evidence badges pointing to GlyGen dataset, used for sources without a url|
|PMID|PubMed ID for files in which all entries are associated with one publication|
|PMID field|Field where PMID can be located for files that contain records from multiple publications|
|Notes|Misc notes field|

Updates for 2.5 release:
------
1. Updated UnicarbKB dataset IDs (GLY_000040:Human|GLY_000040:Mouse --> GLY_000040:Human|GLY_000041:Mouse)
2. New download files added: matrixdb_CORE.tab, glyconnect_chicken.json, chicken_o_glcnacome_mcw.csv, ccRCC_TMT_intact_glycopeptide_abundance_MD-MAD.tsv, diabetes_glycomic_mapping.csv, and Custom_MatrixDB_biomolecules.tsv
3. Added Pig dataset ID to OGlcNAcAtlas rows 
4. Switched doi link from "Notes" to "PMID" column for glygen_upload.csv
5. Updated ambiguous_sites.csv and unambiguous_sites.csv name and added chicken  
6. Updated "PMID" header to "Publication" and provided corresponding key:value for entries with literature 

Updates for 2.4 release:
------
1. Updated all paths to 'current' folder
2. Added species to GlyGen dataset ID
3. Added PMID field
4. Added Notes field
5. Removed files without GlyTouCan accessions
6. Added new files: glyconnect_pig.json, glygen_upload.csv
