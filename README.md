# species2taxid.py
Fetches the NCBI TaxID and full taxonomy from list of species names.

usage:
species2taxid.py list-of-species.txt outputfile.txt tax2lin.txt "Viridiplantae"

The list of species should be genus and species names separated by a white space.
tax2lin.txt is a local list of NCBI plant species and their TaxIDs and taxonomy. For other kingdoms, or if you want to only use most recent names, this file can be started from scratch. Building this file will take some time because each entry must be downloaded from NCBI. Retain the file for future use, it is updated with each run with any species not previously searched.
