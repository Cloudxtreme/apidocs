<!-- toc -->
## j.tools.performancetrace

- /opt/jumpscale7/lib/JumpScale/baselib/performancetrace/PerformanceTrace.py

### Methods

    

#### def profile 

##### arguments

- methodstatement
- locals = \{\}
- globals = \{\}

##### comments

```
create a wrapper method which has no args and then pass that wrapper method to this method
    as first arg
method is passed as a string e.g. 'listDirTest()'
it remove stats is False the path where the stats are will be returned
make sure that whatever arguments used in the statement are passed to the globals

example:

import JumpScale.baselib.performancetrace
do=j.tools.performancetrace.profile('test0b()', globals=globals())

```

