# Resume Parser CLI
A simple Node.js CLI for parse a resume.

This package is pretty much obsolete. I recommend you to switch to [ResumeParser.js](https://github.com/RobyFerro/ResumeParser.js.git), which covers the same functionality as Resume Parser CLI.

## Getting started
```
npm install -g resume-parser-cli
```

#### Usage

```
rparse -f <file> <option>
```

### Options
```
rparse -f <filename> <option>
```
```
     -V, --version         output the version number
     -f, --file [value]    REQUIRED: Add file to parse.
     --export-dir [value]  Select output dir for exported results.
     -t, --text            Get document text
     -i, --images          Find faces inside document
     -p, --pdf             Convert document in pdf
     -c, --clear           Clear result directory
     -j, --json            Export result as JSON
     -s, --show            Show progress in console
     -h, --help            output usage information
```

#### In case of error
If you throw some problem during the installation make sure to grant the right permission in node with this commands
```
npm config set user 0
npm config set unsafe-perm true
```

## Requirements
* Node 10.04.*
* Libreoffice

### Linux dependencies
##### cmake 
###### Fedora:
    yum install cmake
###### Debian:
    apt-get install cmake
##### libopenblas-dev
OPTIONAL Install for improve CPU performance during face recognition:  
###### Fedora:
    yum install openblas-devel.x86_64
###### Debian: 
    sudo apt-get install libopenblas-dev
##### libx11 (XQuartz on OSX)
###### Fedora:
    yum install libX11-devel.x86_64
###### Debian:
    sudo apt-get install libx11-dev
##### libpng 
###### Fedora:
    yum install libpng-devel
###### Debian:
    sudo apt-get install libpng-dev
##### pdftotext 
###### Fedora: 
    yum install poppler-utils
###### Debian:
    sudo apt-get install poppler-utils
##### antiword 
###### Fedora:
    wget https://forensics.cert.org/cert-forensics-tools-release-el7.rpm
    rpm -Uvh cert-forensics-tools-release*rpm
    yum --enablerepo=forensics install antiword
###### Debian: 
    sudo apt-get install antiword
##### unrtf
###### Fedora:
    yum install unrtf
###### Debian:
    sudo apt-get install unrtf
##### tesseract 
###### Fedora:
    yum install tesseract
###### Debian:
    sudo apt-get install tesseract-ocr

