# species2taxid.py
Fetches the NCBI TaxID and full taxonomy from list of species names.

usage:
species2taxid.py list-of-species.txt outputfile.txt tax2lin.txt "Viridiplantae"

You must enter your Entrez email and api key on lines 13 and 15 of the script. See https://ncbiinsights.ncbi.nlm.nih.gov/2017/11/02/new-api-keys-for-the-e-utilities/

The list of species should be genus and species names separated by a white space.
tax2lin.txt is a local list of NCBI plant species and their TaxIDs and taxonomy. For other kingdoms, or if you want to only use most recent names, this file can be started from scratch. Building this file will take some time because each entry must be downloaded from NCBI. Retain the file for future use, it is updated with each run with any species not previously searched.
"Viridiplantae" is an optional extra term to avoid confusion of species names being the same across kingdoms. Other search terms can be added here, e.g. "Viridiplantae NOT Chlorophyta".
