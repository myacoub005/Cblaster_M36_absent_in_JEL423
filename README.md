# Cblaster_M36_absent_in_JEL423

We want to define the unity across all M36 sites in all strains

We have already defined the M36s in terms of JEL423. I have subtracted those hits from the hmmsearch results.
We now have approximately 4 M36s/strain remaining

######Automatically Generate the query files
For every M36 hit from a hmmsearch generate a gbk query file including its supercontig number, 2 flanking genes on either side, and their      start:start.
02.OZ has 4 M36s not found in JEL423. We can start by making query files for each of those. 
Write a program to get the flanking genes, get boundaries (start:stop), and supercontig number.
Output to genbank format with a specific identifier. (i.e. 02.OZ|000530_query.gbk)

######Cblaster search
Perform a cblaster search for every query file against every strain.
run searches in parrallel for each strain. Run the strains sequentially.
Save hits to each loci in a corresponding folder (i.e. 02.OZ|000530_hits/CLFT001_binary.csv).
Any hits in a new strain get cross referenced against the searches already performed (this way we don't need to repeat entire search).

Subtract these results from the list of remaining M36s not found in JEL423. Proceed until all M36s have been assigned. 
  
