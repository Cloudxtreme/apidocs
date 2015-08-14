## j.codetools.regex

- /opt/jumpscale7/lib/JumpScale/baselib/regextools/RegexTools.py
- Properties
    - templates

### def processLines(text,includes="",excludes="") (l253)

includes happens first
excludes last
both are arrays

### def matchMultiple(patterns,text) (l106)

see if any patterns matched
if patterns=[] then will return False

### def findLine(regex,text) (l296)

returns line when found
@param regex is what we are looking for
@param text, we are looking into

### def findOne(pattern,text, flags=0) (l153)

Searches for a one match only on pattern inside text, will throw a RuntimeError if more than one match found
@param pattern: Regex pattern to search for
@param text: Text to search in

### def extractFirstFoundBlock(text,blockStartPatterns,blockStartPatternsNegative=[],blockStopPatterns=[],blockStopPatternsNegative=[],linesIncludePatterns=[".*"],linesExcludePatterns=[],includeMatchingLine=True) (l330)

### def getRegexMatches(pattern, text, flags=0) (l189)

match all occurences and find start and stop in text
return RegexMatches  (is array of RegexMatch)

### def extractBlocks(text,blockStartPatterns=['.*'],blockStartPatternsNegative=[],blockStopPatterns=[],blockStopPatternsNegative=[],linesIncludePatterns=[".*"],linesExcludePatterns=[],includeMatchingLine=True) (l338)

look for blocks starting with line which matches one of patterns in blockStartPatterns and not matching one of patterns in blockStartPatternsNegative
block will stop when line found which matches one of patterns in blockStopPatterns and not in blockStopPatternsNegative or when next match for start is found
in block lines matching linesIncludePatterns will be kept and reverse for linesExcludePatterns
example pattern: '^class ' looks for class at beginning of line with space behind

### def getRegexMatch(pattern, text, flags=0) (l225)

find the first match in the string that matches the pattern.
@return RegexMatch object, or None if didn't match any.

### def yieldRegexMatches(pattern, text, flags=0) (l202)

The same as getRegexMatches but instead of returning a list that contains all matches it uses yield to return a generator object
witch would improve the performance of the search function.

### def findHtmlBlock(subject,tofind,path,dieIfNotFound=True) (l79)

only find 1 block ideal to find e.g. body & header of html doc

### def replaceLines(replaceFunction,arg,text,includes="",excludes="") (l271)

includes happens first (includes of regexes eg @process.* matches full line starting with @process)
excludes last
both are arrays
replace the matched line with line being processed by the functionreplaceFunction(arg,lineWhichMatches)
the replace function has 2 params, argument & the matching line

### def replace(regexFind,regexFindsubsetToReplace,replaceWith,text) (l131)

Search for regexFind in text and if found, replace the subset regexFindsubsetToReplace of regexFind with replacewith and returns the new text
Example:
    replace("Q-Layer Server", "Server", "Computer", "This is a Q-Layer Server")
    will return "This is a Q-Layer Computer"
@param regexFind: String to search for, can be a regular expression
@param regexFindsubsetToReplace: The subset within regexFind that you want to replace
@param replacewith: The replacement
@param text: Text where you want to search and replace

### def findHtmlElement(subject,tofind,path,dieIfNotFound=True) (l68)

### def matchAllText(pattern,text) (l218)

### def getINIAlikeVariableFromText(variableName,text,isArray=False) (l305)

e.g. in text
'
test= something
testarray = 1,2,4,5
'
getINIAlikeVariable("test",text) will return 'something'
@isArray when True and , in result will make array out of 
getINIAlikeVariable("testarray",text,True) will return [1,2,4,5]

### def removeLines(pattern,text) (l244)

remove lines based on pattern

### def findAll(pattern,text, flags=0) (l174)

Search all matches of pattern in text and returns an array
@param pattern: Regex pattern to search for
@param text: Text to search in

### def match(pattern,text) (l91)

search if there is at least 1 match

