# How to develop in mu repository?

## Separate branch
 Create a separate branch for a bigger chunk of task and work on the branch. <br/>
 Run "make all" to see if local build passes. <br/>
 Commit the local changes to the remote branch (git push -u origin <branch-name>) <br/>
 Check with Riad to see if the changes are good and also see if Travis CI build passes. <br/>
 Then attempt to do git merge from branch to master and check if Travis CI build passes. <br/>
 
## Lambdaize {code} <br/>
 Look into the directory : mu/src/lambdaize. This has all the code to lambaize a functionality <br/>
 lambaize/ <br/>
    libmu                         : Library for lambaize - handlers, state machine, defs, wrappers, server, sockets, util <br/>
    test                          : Testing the libmu code <br/>
    lambda_function_template.py   : This piece of code runs in AWS Lambda - has the lambda_handler function <br/>
    lambda_state_server.py        : Basic skeleton of a server - server config and sockets <br/>
    lambdaize.sh                  : Given a function as executable, creates a AWS Lambda function with parameters specified <br/>
    *_server.py                   : Implements specific state machine and server config inherited from infra piece of code, Runs inside AWS Lambda <br/>
    
 
