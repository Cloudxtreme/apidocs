## j.console

- /opt/jumpscale7/lib/JumpScale/core/Console.py
- Properties
    - width
    - indent

class which groups functionality to print to a console
self.width=120
self.indent=0 #current indentation of messages send to console
self.reformat=False #if True will make sure message fits nicely on screen

### def enableOutput() (l653)

### def echo(msg,indent=None,withStar=False,prefix="",log=False,lf=True) (l125)

Display some text to the end-user, use this method instead of print
@param indent std, will use indent from console object (same for all), this param allows to overrule
        will only work when j.console.reformat==True

### def formatMessage(message,prefix="",withStar=False,indent=0,width=0,removeemptylines=True) (l77)

Reformat the message to display to the user and calculate length
@param withStar means put * in front of message
@returns: Length of last line and message to display
@rtype: tuple<number, string>

### def rawInputPerChar(callback,params) (l31)

when typing, char per char will be returned

### def echoListItem(msg) (l149)

Echo a list item
@param msg: Message to display

### def askChoice(choicearray, descr="", sort=True,maxchoice=25,height=30,autocomplete=False) (l399)

@param choicearray is list or dict, when dict key needs to be the object to return,
       the value of the dics is what needs to be returned, the key is the str representation

### def printOutput() (l650)

### def askIntegers(question, invalid_message="invalid input please try again.", min=None, max=None) (l356)

Ask the user for multiple integers

@param question: question that will be echoed before the user needs to input integers
@type question: string
@param invalid_message: message that will be echoed when the user inputs a faulty value
@type invalid_message: string
@param min: optional minimal value for input values, all returned values will be at least min
@type min: number or None
@param max: optional maximal value for input values, all returned values will be at least max
@type max: number of None
@return: the input numbers
@rtype: list<number>

### def echoDict(dictionary,withStar=False,indent=None) (l185)

### def echoListItems(messages, sort=False) (l156)

Echo a sequence (iterator, generator, list, set) as list items

@param messages: messages that need to be written to the console as list items
@type messages: iterable
@param sort: sort the messages before echoing them
@type sort: bool
@param loglevel: Log level
@type loglevel: number

### def hideOutput() (l647)

### def transformDictToMessage(dictionary,withStar=False,indent=None) (l192)

### def askPassword(question, confirm=True, regex=None, retry=-1, validate=None) (l240)

Present a password input question to the user

@param question: Password prompt message
@param confirm: Ask to confirm the password
@type confirm: bool
@param regex: Regex to match in the response
@param retry: Integer counter to retry ask for respone on the question
@param validate: Function to validate provided value

@returns: Password provided by the user
@rtype: string

### def showArray(array,header=True) (l656)

### def echoListWithPrefix(messages,prefix) (l178)

print messages

### def askMultiline(question, escapeString='.') (l623)

Ask the user a question that needs a multi-line answer.

@param question: The question that should be asked to the user
@type question: string
@param escapeString: Optional custom escape string that is used by the user to indicate input has ended.
@type escapeString: string
@return: string multi-line reply by the user, always ending with a newline

### def askString(question, defaultparam='', regex=None, retry=-1, validate=None) (l205)

Get a string response on a question

@param question: Question to respond to
@param defaultparam: Default response on the question if response not passed
@param regex: Regex to match in the response
@param retry: Integer counter to retry ask for respone on the question
@param validate: Function to validate provided value

@returns: Response provided by the user
@rtype: string

### def askInteger(question, defaultValue = None, minValue = None, maxValue = None, retry = -1, validate=None) (l285)

Get an integer response on asked question

@param question: Question need to get response on
@param defaultparam: default response on the question if response not passed
@param minValue: minimum accepted value for that integer
@param maxValue: maximum accepted value for that integer
@param retry: int counter to retry ask for respone on the question
@param validate: Function to validate provided value

@return: integer representing the response on the question

### def askChoiceMultiple(choicearray, descr=None, sort=True) (l592)

### def askYesNo(message="") (l332)

Display a yes/no question and loop until a valid answer is entered

@param message: Question message
@type message: string

@return: Positive or negative answer
@rtype: bool

### def askArrayRow(array,header=True,descr="",returncol=None) (l691)

### def echoWithPrefix(message,prefix,withStar=False,indent=None) (l172)

print a message which is formatted with a prefix

### def showOutput() (l644)

### def cls() (l199)

clear screen

