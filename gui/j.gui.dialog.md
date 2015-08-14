## j.gui.dialog

- /opt/jumpscale7/lib/JumpScale/core/gui/dialog/EasyDialog.py
- Properties
    - easyDialog

### def navigateTo(url) (l247)

### def askChoice(question, choices, defaultValue = None, pageSize = 10, sortChoices=False, sortCallBack=None) (l161)

Ask the user the supplied question and list the choices to choose from, if no response given the default value is used

@param question: question to be display to the user
@param choices: list of choices for the user to choose from
@param defaultValue: the value that will be used if no response given
@param pageSize: max number of choices that can be prompted to the user in a single screen
@param sortChoices: if True, choices will be sorted before showing them to the user
@param sortCallBack: A callback function to handle the sorting of the choices (will only be used if sortChoices is set to True)

@return:  selected choice

### def showProgress(minvalue, maxvalue, currentvalue) (l231)

Shows a progress bar according to the given values

@param minvalue: minVlue of scale
@param maxvalue: maxvlaue of scale
@param currentvalue: the current value to show the progress

### def askChoiceMultiple(question, choices, defaultValue = None, pageSize = 10, sortChoices=False, sortCallBack=None) (l177)

Ask the user the supplied question and list the choices to choose from, if no response given the default value[s] is used

@param question: question to be display to the user
@param choices: list of choices for the user to choose from
@param defaultValue: default value assumed if no user response is given, default value can be a single value or a comma separated list of values
@param pageSize: max number of choices that can be prompted to the user in a single screen
@param sortChoices: if True, choices will be sorted before showing them to the user
@param sortCallBack: A callback function to handle the sorting of the choices (will only be used if sortChoices is set to True)

@return:  selected choice[s] or default value[s]

### def askMultiline(question, defaultValue=None) (l193)

Asks the user the supplied question, where the answer could be multi-lines

@param question: the question to be displayed

### def pm_setDialogHandler() (l44)

### def askDirPath(message, startPath = None) (l93)

Prompts for a selection of a file path starting from startPath if given and '/' if not

@param message: message that would be displayed to the user above the selection menu
@param startPath: base dir of the navigation tree
@return: path to the directory selected

### def askDate(question, minValue = None, maxValue = None, selectedValue = None, format = 'YYYY/MM/DD') (l202)

Asks user a question that its answer is a date between minValue and maxValue

Note: this note my seem out of place, but is is important to note that currently in the EasyDialogConsole implementation only dates with format YYYY/MM/DD are supported

@param question: question that will be prompted to the user
@param minValue: optional value for the lower boundary date
@param maxValue: optional value for the upper boundary date
@param selectedValue:
@param  format: the format of the input date

### def askIntegers(question) (l151)

Asks user the supplied question and prompt for an answer

@param question: question to be prompted
@return: response integer

### def clear() (l253)

### def chooseDialogType(type) (l50)

supported types today: console,win32,wizardserver
@param type DialogType enumerator

### def askString(question, defaultValue = None, validator=None) (l107)

Asks the user the supplied question and prompt for an answer, if none given the default value is used
@param question: question to be displayed
@param defaultValue: if the user did not provide a response this value is used as an answer
@param validator: regex validation value
@return: response string or the default value

### def askForm(form) (l250)

### def askDateTime(question, minValue = None, maxValue = None, selectedValue = None, format = 'YYYY/MM/DD hhmm') (l217)

Asks user a question that its answer is a datetime between minValue and maxValue

Note: this note my seem out of place, but is is important to note that currently in the EasyDialogConsole implementation only dates with format YYYY/MM/DD are supported

@param question: question that will be prompted to the user
@param minValue: optional value for the lower boundary date
@param maxValue: optional value for the upper boundary date
@param selectedValue:
@param  format: the format of the input date

### def askInteger(question, defaultValue = None) (l139)

Asks user the supplied question and prompt for an answer, if none given the default value is used, the response and the default value must be valid integer

@param question: question to be displayed
@param defaultValue: if the user did not provide a response this value is used as an answer
@return: response integer or the default value

### def showLogging(text) (l241)

Shows logging message

### def message(message) (l70)

prints the given message to the screen

@param message: message to print

### def askFilePath(message, startPath = None) (l79)

Prompts for a selection of a file path starting from startPath if given and '/' if not

@param message: message that would be displayed to the user above the selection menu
@param startPath: base dir of the navigation tree
@return: path to the file selected

### def showMessageBox(message, title, msgboxButtons = "OK", msgboxIcon = "Information", defaultButton = "OK") (l256)

Shows a large message box

@param message: message for the messagebox
@param title: title of the messagebox
@param msgboxButtons: buttons to show in the messagebox. Possible values are 'OKCancel', 'YesNo', 'YesNoCancel', 'OK'
@param msgboxIcon: icon to show in the messagebox. Possible values are 'None', 'Error', 'Warning', 'Information', 'Question'
@param defaultButton: default button for the messagebox. Possible values are 'OK', 'Cancel', 'Yes', 'No'

@return: A JSON encoded string containing the selected button clicked

### def askYesNo(question, defaultValue = None) (l118)

Asks user the supplied question and prompt for an answer, if none given the default value is used, the response and the default value one of the values [y|Y|yes|Yes..n|N|No..]

Note:For the EasyDialogConol implementation, currently the default value effect is ignored since it would require changing the jumpscale vapp
@param question: question to be prompted
@param defaultValue: if the user did not provide a response this value is used as an answer
@return: response answer or the default value

### def askPassword(question, confirm=True, regex=None, retry=-1, defaultValue=None) (l130)

Asks the supplied question and prompts for password

@param question: question to be displayed
@return: response string

