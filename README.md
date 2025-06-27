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

Updates for 2.9 release:
------
NOTE: The TableMaker datasets are now in CSV format. I promise I will not make additional modifications to the file format moving forward.

1. Updated dataset ID (file name) for TD10901054.txt to TD1468274.csv to reflect the change made on https://glygen.ccrc.uga.edu/tablemaker/. TableMaker team has also addressed the issue of the ID changing when a curator makes modifications to the table. 
2. Added additional TableMaker datasets for human glycans TD1040297.csv, TD2415036.csv, TD2986138.csv, TD4951079.csv, TD7181079.csv, TD7732158.csv, TD8189974.csv, TD8741863.csv
3. Added glycan tissue data from the GlycomeAtlas Dataset (glycosmos_glycomeatlas_list.csv) for human, mouse, and zebrafish. 
4. Added RCSB PDB glycosylation data for Human (glycosites_rcsb_pdb.csv).

Updates for 2.8 release:
------
1. Added filtered_glycoproteins_glycan_list.csv - a resource retreived from GlyCosmos (only GlycoProtDB data isolated) that contains glycosylation site information. Given this file was modified, it lives in the following full path:/data/projects/glygen/generated/datasets/compiled/filtered_glycoproteins_glycan_list.csv. Please let me know if this poses any issues. 
2. Added two TableMaker datasets: TD10901054.txt (fruitfly) and TD1127346.txt (zebrafish)
3. Added hamster files for glyconnect. No zebrafish files available for this resource. 
4. Added zebrafish files for MCW. No hamster files available for this resource. 
5. Note: No zebrafish or hamster files available for O-Glcnac Atlas. Will update if/when data becomes available. 

Updates for 2.7 release:
------
1. Added mw_refmet_mapping_result.tsv - a new resource we are implementing that contains monosaccharide information. Please add the xrefs on your end. 
2. Updated the user submitted data to tsv format: 1-s2.0-S1535947624000070-mmc5.tsv and 1-s2.0-S1535947624000070-mmc7.tsv
3. Added bovine files for glyconnect, mcw, and dataset ID to OGlcNAcAtlas rows.
4. The file previously named allbiomarkers.tsv has been renamed to oncomx.tsv. This change reflects the new organization by the BiomarkerKB team, which now separates their data by resource. The oncomx.tsv file will now include all protein and glycan biomarker data going forward.  

Updates for 2.6 release:
------
1. Please use the SNFG files (PubChem_substance_compound.csv and sia-table2.tsv) to create an SNFG xref file and map these SIDs/CIDs to GlyTouCan. These files also contain names, which you might be able to add to your names.tsv file. Ticket #843 has more information if needed.
2. Added arabidopsis files for glyconnect, mcw, and dataset ID to OGlcNAcAtlas rows.
3. Two new user submitted data added:1-s2.0-S1535947624000070-mmc5.xlsx and 1-s2.0-S1535947624000070-mmc7.xlsx

Updates for 2.5 release:
------
1. Updated UnicarbKB dataset IDs (GLY_000040:Human|GLY_000040:Mouse --> GLY_000040:Human|GLY_000041:Mouse)
2. New download files added: matrixdb_CORE.tab, glyconnect_chicken.json, chicken_o_glcnacome_mcw.csv, ccRCC_TMT_intact_glycopeptide_abundance_MD-MAD.tsv, diabetes_glycomic_mapping.csv, and Custom_MatrixDB_biomolecules.tsv
3. Added Pig dataset ID to OGlcNAcAtlas rows 
4. Switched doi link from "Notes" to "PMID" column for glygen_upload.csv
5. Changed OGlcNAcAtlas file names from ambiguous_sites_version_2.0.csv and unambiguous_sites_version_2.0.csv to ambiguous_sites.csv and unambiguous_sites.csv, respectively. Added chicken  
6. Updated "PMID" header to "Publication" and provided corresponding key:value for entries with literature 
7. Changed BiomarkerKB file name and type from allbiomarkers-all.csv to allbiomarkers.tsv, updated "PMID field"

Updates for 2.4 release:
------
1. Updated all paths to 'current' folder
2. Added species to GlyGen dataset ID
3. Added PMID field
4. Added Notes field
5. Removed files without GlyTouCan accessions
6. Added new files: glyconnect_pig.json, glygen_upload.csv
