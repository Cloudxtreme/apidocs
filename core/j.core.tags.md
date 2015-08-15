## j.core.tags

- /opt/jumpscale7/lib/JumpScale/baselib/tags/TagsFactory.py

### Methods

Factory Class of dealing with TAGS     

#### getObject 
##### arguments

    - tagstring = ''
    - setFunction4Tagstring

##### comments

check whether labelname exists in the labels 

@param tagstring:  example "important customer:kristof"
@type tagstring: string

#### getTagString 
##### arguments

    - labels
    - tags

##### comments

Return a valid tags string, it's recommended to use this function
and not to build the script manually to skip reserved letters.

@param labels: A set of labels
@param tags: A dict with key values

