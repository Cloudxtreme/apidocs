<!-- toc -->
## j.base.byteprocessor

- /opt/jumpscale7/lib/JumpScale/core/BYTEPROCESSOR.py
- Properties
    - hashTiger192
    - hashTiger160
    - compress
    - decompress
    - hashTiger160bin
    - disperse
    - undisperse
    - hashMd5
    - getDispersedBlockObject

### Methods

ByteProcessor

#### def compress 

##### arguments

- s

#### def decompress 

##### arguments

- s

#### def disperse 

##### arguments

- s
- nrblocks
- extrablocks
- compress = True

##### comments

```
returns DispersedBlock object

```

#### def getDispersedBlockObject 

##### arguments

#### def hashMd5 

##### arguments

- s

#### def hashTiger160 

##### arguments

- s

#### def hashTiger160bin 

##### arguments

- s

#### def hashTiger192 

##### arguments

- s

#### def undisperse 

##### arguments

- dispersedBlockObject
- uncompress = True

