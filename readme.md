# Goal

# Initial Data Cleaning
Reduced the file size for the following files:
- title.basics.tsv (929MB) -> title.movies.tsv (55MB) (`grep 'movie' title.basics.tsv > title.movies.tsv` then `head -1 title.basics.tsv | cat - title.movies.tsv > temp && mv temp title.movies.tsv`) 
- title.principals.tsv (3.76GB) -> title.actors.tsv (923MB) (`grep 'actor' title.principals.tsv > title.actors.tsv` then `head -1 title.principals.tsv | cat - title.actors.tsv > temp && mv temp title.actors.tsv`)
- (`grep 'US' title.akas.tsv > title.us.tsv` then `head -1 title.akas.tsv | cat - title.us.tsv > temp && mv temp title.us.tsv`)