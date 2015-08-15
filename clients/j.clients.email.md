<!-- toc -->
## j.clients.email

- /opt/jumpscale7/lib/JumpScale/baselib/mailclient/emailclient.py

### Methods

#### def send 

##### arguments

- recipients
- sender = ''
- subject = ''
- message = ''
- files
- mimetype

##### comments

```
@param recipients: Recipients of the message
@type recipients: mixed, string or list
@param sender: Sender of the email
@type sender: string
@param subject: Subject of the email
@type subject: string
@param message: Body of the email
@type message: string
@param files: List of paths to files to attach
@type files: list of strings
@param mimetype: Type of the body plain, html or None for autodetection
@type mimetype: string

```

