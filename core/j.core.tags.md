## j.core.tags

- /opt/jumpscale7/lib/JumpScale/baselib/tags/TagsFactory.py

Factory Class of dealing with TAGS     

#### def getObject(tagstring="",setFunction4Tagstring=None) 

    check whether labelname exists in the labels 
    
    @param tagstring:  example "important customer:kristof"
    @type tagstring: string

#### def getTagString(labels=None, tags=None) 

    Return a valid tags string, it's recommended to use this function
    and not to build the script manually to skip reserved letters.
    
    @param labels: A set of labels
    @param tags: A dict with key values

