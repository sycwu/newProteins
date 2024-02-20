Overall, the resulting list of novel genes identified is similar to the attempt with v10.0
At best, there are 50 (12 from newproteins + 38 from newProteinsNewTranscript_ListofProteins) new genes - but the final novel list is likely shorter.
This is because there are some genes that have populated pages on Xenbase already (eg. RNASEH1).

**output.txt** 
(n = 309)
this is the raw list of NOVEL proteins that have not been mapped to before by v10.7

**matchedProteins.txt**
(n = 208)
this is a SUBSET of output.txt: braker transcripts which mapped to v10.7 transcripts AND have hits for the corresponding v10.7 query
the majority of braker hits shared gene roots with the corresponding v10.7 hit
*POSSIBLE TODO: compute shared root % and e-value confidence*

**newProteins.txt** 
(n = 18; 12 are unique)
this is a SUBSET of output.txt: braker transcripts which mapped to v10.7 transcripts BUT DON'T have hits for the corresponding v10.7 query
*POSSIBLE TODO: look into pre-existing information on xenbase*

**newProteinsNewTranscript.txt** 
(n = 83)
this is a SUBSET of output.txt: braker transcripts which DID NOT map to v10.7 transcripts

**newProteinsNewTranscript_ListofProteins.txt**
(n = 38)
this is the unique list of proteins in newProteinsNewTranscript.txt
*POSSIBLE TODO: look into pre-existing information on xenbase*

**Source Files**
**ALLbrakerAA against human.txt**
BiSeqLe result from using Braker AA as query, and human genome as reference.
**brakerAA against v10.7.txt**
BiSeqLe result from using Braker AA as query, and Xenopus tropicalis v10.7 as reference.
**v10.7 against human.txt**
BiSeqLe result from using Xenopus tropicalis v.10.7 as query, and human genome as reference.