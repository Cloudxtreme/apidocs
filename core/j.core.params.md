## j.core.params

- /opt/jumpscale7/lib/JumpScale/baselib/params/Params.py

This factory can create new Params objects

    #### def get(dictObject=\{\}) 
    
    Create and return a new Params object
    
    @param dictObject when dict given then dict will be converted into params
    @return: a new Params object
    @rtype: Params
    #### def isParams(p) 
    
    Return if the argument object is an instance of Params
    
    @param p: object to check
    @type p: object
    @return: Whether or not `p` is a Params instance
    @rtype: boolean
