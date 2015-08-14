## j.tools.text

- /opt/jumpscale7/lib/JumpScale/core/system/text.py
- Properties
    - machinetext2val
    - dealWithQuote
    - lstrip
    - pythonObjToStr1line
    - prefix_remove_withtrailing
    - prefix
    - toSafePath
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

### @staticmethod (l535)

do reverse of:
     SPACE -> \S
     " -> \Q
     , -> \K
     : -> \D
     \n -> return

### @staticmethod (l656)

look for 'something,else' the comma needs to be converted to \k

### @staticmethod (l135)

remove all spaces at beginning & end of line when relevant

### @staticmethod (l428)

### @staticmethod (l83)

there can be chars for prefix (e.g. '< :*: aline'  and this function looking for :*: would still work and ignore '< ')
@param onlyPrefix if True means only when prefix found will be returned, rest discarded

### @staticmethod (l60)

### @staticmethod (l19)

process string so it can be used in a path on windows or linux

### @staticmethod (l131)

### @staticmethod (l104)

### @staticmethod (l578)

do reverse of:
            SPACE -> \S
            " -> \Q
            , -> \K
            : -> \D
            
-> \N

### @staticmethod (l505)

'something ' removes ''
all spaces & commas & : inside ' '  are converted
 SPACE -> \S
 " -> \Q
 , -> \K
 : -> \D
 \n -> \N

### @staticmethod (l702)

keys are always treated as string
@type can be int,bool or float (otherwise its always str)

### @staticmethod (l316)

look for \{\{\}\} return as list

### @staticmethod (l636)

### @staticmethod (l68)

@param onlyPrefix if True means only when prefix found will be returned, rest discarded

### @staticmethod (l33)

### @staticmethod (l99)

### @staticmethod (l12)

### @staticmethod (l666)

look for [something,2] the comma needs to be converted to \k

### @staticmethod (l432)

try to convert a python object to string representation works for None, bool, integer, float, dict, list

### @staticmethod (l641)

### @staticmethod (l529)

### @staticmethod (l596)

### @staticmethod (l51)

### @staticmethod (l410)

look for {{}} in code and evaluate as python result is converted back to str

### @staticmethod (l153)

look for @ASK statements in text, where found replace with input from user

syntax for ask is:
    @ASK name:aname type:str descr:adescr default:adefault regex:aregex retry:10 minValue:10 maxValue:20 dropdownvals:1,2,3

    descr, default & regex can be between '' if spaces inside

    types are: str,float,int,bool,dropdown,multiline
    the multiline will open joe as editor

    retry means will keep on retrying x times until ask is done properly

    dropdownvals is comma separated list of values to ask for when type dropdown

@ASK can be at any position in the text

### @staticmethod (l113)

### @staticmethod (l628)

### @staticmethod (l612)

### @staticmethod (l357)

convert list, dict of strings 
or convert 1 string to python objects

### @staticmethod (l676)

@type can be int,bool or float (otherwise its always str)

