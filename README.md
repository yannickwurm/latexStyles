latexStyles
===========

Latex stylings (for main text or bibliography) that have been useful to me.

* Molecular Ecology  (used for http://onlinelibrary.wiley.com/doi/10.1111/j.1365-294X.2010.04561.x/abstract). Build with merlin.mbs. 
* `mine.bst` and `mine-unsrt.bst`   - derived from Mol Ecol. 
* Briefings in Functional Genomicss 
* Genome Research

No guarantees or anything


-- Yannick Wurm - [https://wurmlab.github.io](https://wurmlab.github.io)

=======


## converting from long to short journal names

To change from long to short journal names I use: [https://github.com/wurmlab/bibtexJournalConverter](https://github.com/wurmlab/bibtexJournalConverter)
    
Previously I used: 
      ./build/scripts-2.7/jabbrev.py ~/Dropbox/Papers/PhdBib1.bib examples/journal_abbreviations.txt > ~/Dropbox/Papers/PhdBib1-short.bib

Note - currently jabbrev skips articles that contain an "@" - need to be sure to eliminate those first. !


## Changing numbers of authors shown. 

To change numbers of names shown, need to edit the following lines:
```
nameptr #1 >
        {
          nameptr #3
          #1 + =
          numnames #4
```
e.g. as above: 

 * if num authors > 4 , show only the first 3 then "et al"
 * if num authors <= 4, show all authors. 

