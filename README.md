# Aflie COI training data

These files contain a set of publicaly available DNA barcode sequences obtained from BOLD (http://www.boldsystems.org/index.php).

The filename indicates the kingdom from which the barcode sequences are derivided. Each file contains the following columns of data:
```
processid		- unique ID for relating sequence back to the BOLD database
clean_dna		- the DNA barcode sequence for the specimen
kingdom			- subsequent columns are the taxonomic classifications
phylum	
class	
order	
family	
subfamily	
genus 			
species			- note: this column may be sparsely populated, and is absent for the animal sequences.
```

## Extract the data

The tar.bz2 format was used to get the files compressed so they fit under the 100MB limit of GitHub (not as good as [middle-out compression](http://www.piedpiper.com) but it does the job). 

The following command can be used to decompress the data:

```
#animal
tar -jxvf animal_coi_clean.tar.bz2

#all at once
tar -jxvf *_coi_clean.tar.bz2

```

