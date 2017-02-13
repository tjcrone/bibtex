# BibTex Repository

This is my BibTex repository which contains my primary BibTex database and a Python
script (doi2bib) which converts a DOI into a BibTex entry. The script can operate
with a DOI as the single command line argument or by redirecting a file with a list
of DOIs into the script. The script prints the entry to the screen which can be
redirected into your database.

Here is a simple usage example:

./doi2bib "10.1029/2004GC000905"

This script requires the "unicode_dict.py" file which facilitates the conversion of
special characters into LaTex code.

The script works pretty well, but it's not perfect, in part because the doi.org
database is not perfect. The worst thing it can do is only list the first author,
because some journals only push the first author to the database. It can also add
et al. when the author list is very long, which is also not ideal. So I check the
author list first when using this script.
