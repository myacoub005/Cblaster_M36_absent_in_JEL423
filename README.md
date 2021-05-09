# Cblaster_M36_absent_in_JEL423

Automatically Generate the query files:
  For every M36 hit in a hmmsearch result generate a gbk query file including its supercontig number, 2 flanking genes on either side, and their start:stop

Cblaster search:
  Perform a cblaster search for every query file generated against every strain. 
  For each strain in parallel execute the query for the strain I am running on. 
