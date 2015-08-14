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

    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    
    look for @ASK statements in text, where found replace with input from user
    
    syntax for ask is:
        @ASK name:aname type:str descr:adescr default:adefault regex:aregex retry:10 minValue:10 maxValue:20 dropdownvals:1,2,3
    
        descr, default & regex can be between '' if spaces inside
    
        types are: str,float,int,bool,dropdown,multiline
        the multiline will open joe as editor
    
        retry means will keep on retrying x times until ask is done properly
    
        dropdownvals is comma separated list of values to ask for when type dropdown
    
    @ASK can be at any position in the text
    #### @staticmethod 
    
    look for [something,2] the comma needs to be converted to \k
    #### @staticmethod 
    
    look for 'something,else' the comma needs to be converted to \k
    #### @staticmethod 
    
    look for \{\{\}\} in code and evaluate as python result is converted back to str
    #### @staticmethod 
    #### @staticmethod 
    
    keys are always treated as string
    @type can be int,bool or float (otherwise its always str)
    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    
    @type can be int,bool or float (otherwise its always str)
    #### @staticmethod 
    
    look for \{\{\}\} return as list
    #### @staticmethod 
    
    'something ' removes ''
    all spaces & commas & : inside ' '  are converted
     SPACE -> \S
     " -> \Q
     , -> \K
     : -> \D
     \n -> \N
    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    
    remove all spaces at beginning & end of line when relevant
    #### @staticmethod 
    
    do reverse of:
                SPACE -> \S
                " -> \Q
                , -> \K
                : -> \D
                
    -> \N
    #### @staticmethod 
    
    do reverse of:
         SPACE -> \S
         " -> \Q
         , -> \K
         : -> \D
         \n -> return
    #### @staticmethod 
    #### @staticmethod 
    
    @param onlyPrefix if True means only when prefix found will be returned, rest discarded
    #### @staticmethod 
    
    there can be chars for prefix (e.g. '< :*: aline'  and this function looking for :*: would still work and ignore '< ')
    @param onlyPrefix if True means only when prefix found will be returned, rest discarded
    #### @staticmethod 
    
    try to convert a python object to string representation works for None, bool, integer, float, dict, list
    #### @staticmethod 
    #### @staticmethod 
    #### @staticmethod 
    
    convert list, dict of strings 
    or convert 1 string to python objects
    #### @staticmethod 
    #### @staticmethod 
    
    process string so it can be used in a path on windows or linux
    #### @staticmethod 
    #### @staticmethod 
