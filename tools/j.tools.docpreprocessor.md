## j.tools.docpreprocessor

- /opt/jumpscale7/lib/JumpScale/portal/docpreprocessor/DocPreprocessorFactory.py

### def generateFromDir(path, macrosPaths=[], visibility=[], cacheDir="") (l67)

@param path is starting point, will look for generate.cfg & params.cfg in this dir, input in these files will determine how preprocessor will work
@param macrosPaths are dirs where macro's are they are in form of tasklets
@param cacheDir if non std caching dir override here

### def getMacroPath() (l123)

### def generate(preprocessorobject, outpath="out", startDoc="Home", visibility=[], reset=True, outputdocname="", format="preprocess", deepcopy=False) (l18)

### def get(contentDirs=[], varsPath="", spacename="") (l7)

@param contentDirs are the dirs where we will load wiki files from & parse

