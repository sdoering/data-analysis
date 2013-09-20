datatools
=========

Just a repo for reminding me of datatools and their use


sed:
  * 's/irgendwas/irgendwer/g' # replacing 'irgendwas' with 'irgendwer' everytime it occurs in a document|stream

grep:
  * grep -v 'irgendwas' # show only lines where 'irgendwas' does not occur
  * 

cat: 

head/tail:

wc:
 * -l # count lines
 * 
 
sort:

uniq:

awk:
  * awk 'rand() < 0.1' file.xxx | ... #obtaining a 10% sample from a file
  * awk -F ";" '{ sum += $3 } END { printf "%.2f\n", sum }' # taking the third column (delimiter=';') and summing it. Printing it with a precision of 2 digits

make: 
  * use to reccord workflows when having to do the same analysis more than once
  * 
  
python:
  Good for more complex analysis
  * ipython(!!!)
  * 
  
  * pandas
  * csv
  * MySQL
  * sqlite3
  * import tablib
  * import requests
  * import dataset
  * import nltk
  * import BeautifulSoup
  * 
  
links:
 * [http://www.gregreda.com/2013/07/15/unix-commands-for-data-science/](http://www.gregreda.com/2013/07/15/unix-commands-for-data-science/)
 * [http://jeroenjanssens.com/2013/09/19/seven-command-line-tools-for-data-science.html](http://jeroenjanssens.com/2013/09/19/seven-command-line-tools-for-data-science.html)
 * [https://news.ycombinator.com/item?id=6412190](https://news.ycombinator.com/item?id=6412190)
