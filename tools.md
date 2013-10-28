datatools
=========

##Just a repo for reminding me of datatools and their use


**sed:**
  * 's/irgendwas/irgendwer/g' # replacing 'irgendwas' with 'irgendwer' everytime it occurs in a document|stream

**grep:**
  * grep -v 'irgendwas' # show only lines where 'irgendwas' does not occur
  * 

**cat:**

**head/tail:**

**wc:**
 * -l # count lines
 * 
 
**sort:**

**uniq:**

**awk:**
  * awk 'rand() < 0.1' file.xxx | ... #obtaining a 10% sample from a file
  * awk -F ";" '{ sum += $3 } END { printf "%.2f\n", sum }' # taking the third column (delimiter=';') and summing it. Printing it with a precision of 2 digits
  * will print all but very first column:
    + cat somefile | awk '{$1=""; print $0}'    
  * will print all but two first columns:
    + cat somefile | awk '{$1=$2=""; print $0}'
  * check if one (or multiple) conditions are met:
    + awk -F ';' '($2 == "ABCD") && ($3 == "MNOP") && ($4 == "KLPM") { print $2, $3;}'  file.xml
  * show last two columns:
    + awk '{print $(NF-1),"\t",$NF}' file
  * If, else if && else:
    +  awk '{if ($5 == "pictureshow"); else if ($6 == "artikel" || $7 == "artikel" || $8 == "artikel" || $9 == "artikel") ; else print $0}'
    +  == : equals
    +  ~ : is like

**make:**
  * use to reccord workflows when having to do the same analysis more than once
  * 
  
**Shell Scripting**
  * [testing exit values](blog.sanctum.geek.nz/testing-exit-values-bash/)

**MySQL**
  * This will create a tab-separated file, each row on its own line. To alter this behavior, it is possible to add modifiers to the query:
 
    SELECT id,product_name FROM orders
    INTO OUTFILE '/tmp/orders.csv'
    FIELDS TERMINATED BY ','
    ENCLOSED BY '"'
    LINES TERMINATED BY '\n'

**python:**
  Good for more complex analysis
  * [ipython](http://ipython.org/)!!!
  * [pandas](http://pandas.pydata.org/)
  * [csv](http://docs.python.org/2/library/csv.html)
  * [MySQL](https://code.google.com/p/pymysql/)
  * [sqlite3](http://docs.python.org/2/library/sqlite3.html)
  * [tablib](https://github.com/kennethreitz/tablib)
  * [requests](https://github.com/kennethreitz/requests)
  * [nltk](http://nltk.org/)
  * [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/)
  * [dataset](http://dataset.readthedocs.org/en/latest/quickstart.html#reading-data-from-tables)
  * [python guide](https://github.com/kennethreitz/python-guide)
  * 
  
**links:**
 * [http://www.gregreda.com/2013/07/15/unix-commands-for-data-science/](http://www.gregreda.com/2013/07/15/unix-commands-for-data-science/)
 * [http://jeroenjanssens.com/2013/09/19/seven-command-line-tools-for-data-science.html](http://jeroenjanssens.com/2013/09/19/seven-command-line-tools-for-data-science.html)
 * [https://news.ycombinator.com/item?id=6412190](https://news.ycombinator.com/item?id=6412190)
 * [short statistical tutorials](http://www.autonlab.org/tutorials/)
