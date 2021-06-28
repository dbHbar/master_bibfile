# master_bibfile
This repository contains the master bibfile to be used, nurtured and synced over different paper projects.  
To use it, git clone this repository to a local folder on your
machine, preferably a directory called bibfile_master parallel to the
one where you edit a paper´s latex file, since in the papers's
texfile we call it as ../bibfile_master/mybibs_bt, and it would be
good if we don't have to edit that line all the time between different
versions of different contributors.    
To add your own bib-entries, first pull the latest version, then edit locally, and then git add "mybibs_bt", git commit -m "some meaningful message about changes you made", and git push it back to the online repository.  

IMPORTANT: 
1. to avoid bibtex errors due to double entries, please verify that
the entry is not yet present yet in the bibtex file - or at least not
the same bibtex-entry. 
2. Please add only "clean" entries to the bib-tex file.  No weird
characters,  non iso-encodings etc that later create problems when
latexing.  It is also good practice to delete ISSN and URL entries
from these bib-entries, as current standard revtex4 settings don't
take those out and create a messy library. 
3. Please DO NOT use editors that introduce additional line break symbols.  In emacs they show up as thousands of ^M symbols, one at the end of each line and make for a file that github considers as completely different, with no chance to automatically merge edits!