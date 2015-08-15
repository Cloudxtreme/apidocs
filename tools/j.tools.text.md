<!-- toc -->
## j.tools.text

- /opt/jumpscale7/lib/JumpScale/core/system/text.py
- Properties
    - machinetext2val
    - dealWithQuote
    - lstrip
    - pythonObjToStr1line
    - wrap
    - prefix_remove_withtrailing
    - prefix
    - toSafePath
    - strip
    - isNumeric
    - addTimeHR
    - machinetext2str
    - hrd2machinetext
    - getDict
    - getMacroCandidates
    - isInt
    - prefix_remove
    - toAscii
    - addCmd
    - pythonObjToStr
    - dealWithList
    - toStr
    - getBool
    - getFloat
    - toUnicode
    - eval
    - ask
    - addVal
    - isFloat
    - replaceQuotes
    - str2var
    - getInt
    - getList

### Methods

#### def addCmd 

##### arguments

- out
- entity
- cmd

#### def addTimeHR 

##### arguments

- line
- epoch
- start = 50

#### def addVal 

##### arguments

- out
- name
- val
- addtimehr = False

#### def ask 

##### arguments

- content
- name
- args = \{\}
- ask = True

##### comments

```
look for @ASK statements in text, where found replace with input from user

syntax for ask is:
    @ASK name:aname type:str descr:adescr default:adefault regex:aregex retry:10
    minValue:10 maxValue:20 dropdownvals:1,2,3

    descr, default & regex can be between '' if spaces inside

    types are: str,float,int,bool,dropdown,multiline
    the multiline will open joe as editor

    retry means will keep on retrying x times until ask is done properly

    dropdownvals is comma separated list of values to ask for when type dropdown

@ASK can be at any position in the text

```

#### def dealWithList 

##### arguments

- text

##### comments

```
look for [something,2] the comma needs to be converted to \k

```

#### def dealWithQuote 

##### arguments

- text

##### comments

```
look for 'something,else' the comma needs to be converted to \k

```

#### def eval 

##### arguments

- code

##### comments

```
look for \{\{\}\} in code and evaluate as python result is converted back to str

```

#### def getBool 

##### arguments

- text

#### def getDict 

##### arguments

- text
- ttype
- deserialize = False

##### comments

```
keys are always treated as string
@type can be int,bool or float (otherwise its always str)

```

#### def getFloat 

##### arguments

- text

#### def getInt 

##### arguments

- text

#### def getList 

##### arguments

- text
- ttype
- deserialize = False

##### comments

```
@type can be int,bool or float (otherwise its always str)

```

#### def getMacroCandidates 

##### arguments

- txt

##### comments

```
look for \{\{\}\} return as list

```

#### def hrd2machinetext 

##### arguments

- value
- onlyone = False

##### comments

```
'something ' removes ''
all spaces & commas & : inside ' '  are converted
 SPACE -> \S
 " -> \Q
 , -> \K
 : -> \D
 \n -> \N

```

#### def isFloat 

##### arguments

- text

#### def isInt 

##### arguments

- text

#### def isNumeric 

##### arguments

- txt

#### def lstrip 

##### arguments

- content

##### comments

```
remove all spaces at beginning & end of line when relevant

```

#### def machinetext2str 

##### arguments

- value

##### comments

```
       do reverse of:
            SPACE -> \S
            " -> \Q
            , -> \K
            : -> \D

-> \N

```

#### def machinetext2val 

##### arguments

- value

##### comments

```
do reverse of:
     SPACE -> \S
     " -> \Q
     , -> \K
     : -> \D
     \n -> return

```

#### def prefix 

##### arguments

- prefix
- txt

#### def prefix_remove 

##### arguments

- prefix
- txt
- onlyPrefix = False

##### comments

```
@param onlyPrefix if True means only when prefix found will be returned, rest discarded

```

#### def prefix_remove_withtrailing 

##### arguments

- prefix
- txt
- onlyPrefix = False

##### comments

```
there can be chars for prefix (e.g. '< :*: aline'  and this function looking for :*: would
    still work and ignore '< ')
@param onlyPrefix if True means only when prefix found will be returned, rest discarded

```

#### def pythonObjToStr 

##### arguments

- obj
- multiline = True
- canBeDict = True
- partial = False

##### comments

```
try to convert a python object to string representation works for None, bool, integer,
    float, dict, list

```

#### def pythonObjToStr1line 

##### arguments

- obj

#### def replaceQuotes 

##### arguments

- value
- replacewith

#### def str2var 

##### arguments

- string

##### comments

```
convert list, dict of strings
or convert 1 string to python objects

```

#### def strip 

##### arguments

- content

#### def toAscii 

##### arguments

- value
- maxlen = 0

#### def toSafePath 

##### arguments

- txt
- maxlen = 0

##### comments

```
process string so it can be used in a path on windows or linux

```

#### def toStr 

##### arguments

- value
- codec = 'utf-8'

#### def toUnicode 

##### arguments

- value
- codec = 'utf-8'

#### def wrap 

##### arguments

- txt
- length = 80

