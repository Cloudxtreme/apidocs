    #### def Object(type_, **kwargs) 
    
    Generic descriptor generator for custom object types
    
    You should be aware this is, unlike non-generic basetypes, a function
    generating a class instance, not a class.
    
    @param type_: Type of which values should be instances
    @type type_: class or type
    @param kwargs: Kwargs sent to L\{jumpscale.pmtypes.base.BaseType.__init__\}
    
    @returns: An instance of a custom descriptor class
    @rtype: L\{jumpscale.pmtypes.base.BaseType.__init__\}
    
    @see: L\{jumpscale.pmtypes.base.BaseType.__init__\}
