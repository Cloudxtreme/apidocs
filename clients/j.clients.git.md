<!-- toc -->
## j.clients.git

- /opt/jumpscale7/lib/JumpScale/baselib/git/GitFactory.py

### Methods

#### def find 

##### arguments

- account
- name
- interactive = False
- returnGitClient = False

##### comments

```
walk over repo's known on system
2 locations are checked
    ~/code
    /opt/code

```

#### def get 

##### arguments

- basedir

##### comments

```
PLEASE USE SSH, see
    http://despiegk.gitbooks.io/jumpscale/content/Howto/how_to_use_git.html for more
    details

```

#### def log 

##### arguments

- msg
- category = ''
- level = 5

