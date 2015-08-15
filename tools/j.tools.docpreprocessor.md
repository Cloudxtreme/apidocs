## j.tools.docpreprocessor

- /opt/jumpscale7/lib/JumpScale/portal/docpreprocessor/DocPreprocessorFactory.py

#### generate 
- arguments
    - preprocessorobject
    - outpath = 'out'
    - startDoc = 'Home'
    - visibility = []
    - reset = True
    - outputdocname = ''
    - format = 'preprocess'
    - deepcopy = False
- comments
    

#### generateFromDir 
- arguments
    - path
    - macrosPaths = []
    - visibility = []
    - cacheDir = ''
- comments
    @param path is starting point, will look for generate.cfg & params.cfg in this dir, input in these files will determine how preprocessor will work
    @param macrosPaths are dirs where macro's are they are in form of tasklets
    @param cacheDir if non std caching dir override here

#### get 
- arguments
    - contentDirs = []
    - varsPath = ''
    - spacename = ''
- comments
    @param contentDirs are the dirs where we will load wiki files from & parse

#### getMacroPath 
- arguments
- comments
    

