# Cblaster_M36_absent_in_JEL423

We want to define the unity across all M36 sites in all strains

Automatically Generate the query files:
  For every M36 hit in a hmmsearch result generate a gbk query file including its supercontig number, 2 flanking genes on either side, and their start:stop

Cblaster search:
  Perform a cblaster search for every query file against every strain. 
  For each strain in parallel execute the query for the strain I am running on.
  Save each of those output files in a particular folder under a specific scheme so that we can know we’ve already run it. 
    i.e. M36_1, M36_2, etc.
  Any hits in a new strain get cross referenced against the searches already performed (this way we don't need to repeat entire search)
    If the strain has a locus corresponding to previous results, add the hits to the corresponding folder 
    Generate a new folder If the results in the new strain are not found in the previous search results
  
