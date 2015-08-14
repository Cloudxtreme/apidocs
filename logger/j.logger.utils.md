## j.logger.utils

- /opt/jumpscale7/lib/JumpScale/core/logging/LogHandler.py

Some log related utilities.

#### def trace(level=5, enabled=True) 

Decorator factory. Use enabled to avoid the logging overhead when it's
not needed. Do not the tracing can *not* be enabled or disabled at
runtime.

Typical usage:

TRACING_ENABLED = True

@j.logger.utils.trace(level=3, enabled=TRACING_ENABLED)
def myFunc(arg1, arg2=12):
    ...

@param level: level to log the calls on
@type level: int
@param enabled: whether or not to disable the tracing
@type enabled: boolean
@return: decorator factory
@rtype: callable

