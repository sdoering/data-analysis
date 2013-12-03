##Misc hacking and cool projects, not directly in the typical data-analysis-space:

  + [http://www.aicbt.com/disguise-detection/](http://www.aicbt.com/disguise-detection/)

* n-gram detection in python:

input_list = ['all', 'this', 'happened', 'more', 'or', 'less']

def find_ngrams(input_list, n):

    return zip(*[input_list[i:] for i in range(n)])
