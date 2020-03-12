# Aflie COI training data

These files contain a set of publicly available DNA barcode sequences obtained from [BOLD](http://www.boldsystems.org/index.php), used in the training of the alignment-free, kingdom level taxonomic classifier: [alfie](https://github.com/CNuge/alfie).

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
species			- note: this column may be sparsely populated, not all bold records are ID'ed to a species level
```

## Extract the data

The tar.bz2 format was used to get the files compressed so they fit under the 100MB limit of GitHub (not as good as [middle-out compression](http://www.piedpiper.com) but it does the job). 

Try double clicking the the compressed files to initiate decompression. If that doesn't work, the following command can be used to decompress the data from the command line:

```
#animal
tar -jxvf animal_coi_clean.tar.bz2

#all at once
tar -jxvf *_coi_clean.tar.bz2

```

