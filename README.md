# nastafile

A NNTP Archive to HTML generator. 

## Getting Started

### Get the newsreader library
You'll need to get cl-nntp library. For quicklisp, clone the repo into your local-projects.

``` sh
git clone https://github.com/fade/cl-nntp.git
```

### Load the cl-nntp library in your listener
``` common-lisp
(ql:quickload :cl-nntp)
```

### Set cl-nntp as the package
```
CL-USER> (in-package :cl-nntp)
```
### Connect to the news server
```
NNTP> (connect "news.gmane.io" 119)
-> Connecting to news.gmane.io:119
<- 200 news.gmane.io InterNetNews NNRP server INN 2.6.3 ready (posting ok)
Registering client news.gmane.io:119 
Adding client to *clients*
NIL
```

### Set the current group
```
(group "gmane.lisp.lispworks.general")

