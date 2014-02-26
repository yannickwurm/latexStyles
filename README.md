latexStyles
===========

Latex stylings (for main text or bibliography) that have been useful to me.

* Molecular Ecology  (used for http://onlinelibrary.wiley.com/doi/10.1111/j.1365-294X.2010.04561.x/abstract). Build with merlin.mbs. 
* `mine.bst` and `mine-unsrt.bst`   - derived from Mol Ecol. 

No guarantees or anything


-- Yannick Wurm - http://yannick.poulet.org 

=======
Latex formats that have been useful to me



To change from long to short journal names I use bibstuff. 

      ./build/scripts-2.7/jabbrev.py ~/Dropbox/Papers/PhdBib1.bib examples/journal_abbreviations.txt > ~/Dropbox/Papers/PhdBib1-short.bib

Note - currently jabbrev skips articles that contain an "@" - need to be sure to eliminate those first. !


To change numbers of names shown, need to edit the following lines:
```
nameptr #1 >
        {
          nameptr #3
          #1 + =
          numnames #3
```
e.g. as above it shows the first 3 authors et al.

