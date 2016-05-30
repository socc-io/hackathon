# hackathon
hackathon template (super simple & no install)

# Features

    - Server JSON-api template (sqlite db binded)
    - Client JSON-api template (Android-java, Web-javascript)
    - JSON-api document template
    - Android common template (such as Listveiw, Popup alert, Slide menu, .. etc)
    - Website common template 
    
# Quick start

## Server
    
    # modify db scheme
    vim db-create.py
    python db-create.py
    
    # start server
    cd server/
    ./run-server.sh 8080
    - your server address is [ 221.10.33.23:8080 ]
    
## Client (Android)
    
    # import client-android with android studio
    # run project
    # open slide menu -> click Server-info
    # modify server address 
    # test server access with buttons (Face-book login, db-input test, etc ...)
    
## Client (Web)

    # some one make here please ...


# JSON-api

    <!--send packet-->
    {
        "uid" : "test-id",                           # for only login
        "upasswd" : "test-passwd",                   # for only login
        "ucookie" : "Fa10923",                       # getting from login
        "callback" : "your callback key" ,           # for common callback method
        "method" : "plus",                           # method.py's method
        "arg1" : 10,
        "arg2" : 20,
        "arg3" : 30,
        ...
    }


    <!--receive packet-->
    {
        "ucookie" : "Fa10923",
        "callback" : "your callback key",           
        "return1" : 60,
        ...
    }
    
    
