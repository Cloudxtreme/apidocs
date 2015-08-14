    #### def yieldRegexMatches(pattern, text, flags=0) 
    
    The same as getRegexMatches but instead of returning a list that contains all matches it uses yield to return a generator object
    witch would improve the performance of the search function.
