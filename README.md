latexStyles
===========

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
