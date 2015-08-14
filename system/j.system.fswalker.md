    #### @staticmethod 
    
    Walk through filesystem and execute a method per file and dirname
    
    Walk through all files and folders starting at C\{root\}, recursive by
    default, calling a given callback with a provided argument and file
    path for every file & dir we could find.
    
    To match the function use the callbackForMatch function which are separate for dir or file
    when it returns True the path will be further processed
    when None (function not given match will not be done)
    
    Examples
    ========
    >>> def my_print(path,arg):
    ...     print arg, path
    ...
    #if return False for callbackFunctionDir then recurse will not happen for that dir
    
    >>> def matchDirOrFile(path,arg):
    ...     return True #means will match all
    ...
    
    >>> FSWalker.walkFunctional('/foo', my_print,my_print, 'test:',matchDirOrFile,matchDirOrFile)
    test: /foo/file1
    test: /foo/file2
    test: /foo/file3
    test: /foo/bar/file4
    
    @param root: Filesystem root to crawl (string)
    #@todo complete
