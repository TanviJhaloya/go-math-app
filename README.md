# go-math-app
#go-container-test

```shell
.
|-- Dockerfile
|-- README.md
`-- src
    |-- conf
    |   `-- app.conf
    |-- go.mod
    |-- go.sum
    |-- main.go
    |-- main_test.go
    `-- views
        |-- invalid-route.html
        `-- result.html
        
        
```


-> main.go: The main application file is main.go, located at the src directory. This file contains all the functionality of the app

-> main_test.go: Some of the functionality from main.go is tested using main_test.go

-> views: The views folder contains the view files invalid-route.html and result.html

-> app.conf: The configuration file app.conf is placed in the conf folder. Beego uses this file to customize the application

-> Dockerfile: Multi-Stage Dockerfile is used to build the go container image

## To access this application use:

http://myapp-load-balancer-1345939904.ap-south-1.elb.amazonaws.com/sum/<integer-1/integer-2

http://myapp-load-balancer-1345939904.ap-south-1.elb.amazonaws.com/product/<integer-1/integer-2

### Note: It will throw `Invalid Operation` as the output if we don't use the appropriate endpoints to access the app.
