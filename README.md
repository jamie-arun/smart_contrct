# smart_contrct
This Project Is To Provide Basic UnderStanding About Error Handlers In Solidity And Functions And Use Of Each!!!!

## Description

This Project Goes Through How You Can Use Different Types of Error Handlers In Solidity And Pros And Cons Compared To Each Other There Are Mainly Three Types Of Error Handlers In Solidity Wjich Are Require,Revert,Assert Which Are Explained Detail In Below:

require(): Used to validate certain conditions before further execution of a function. It takes two parameters as an input.
The first parameter is the condition that you want to validate and the second parameter is the message that will be passed back to the caller if the condition fails. If the condition is satisfied, then the execution of the function continues and the execution jumps to the next statement. 

However, if the condition fails, then the function execution is terminated and the message (the second parameter) is displayed in the logs. The second parameter, however, is optional. require() will work even if you pass only parameter, that is, the condition to be checked. The require() statement is defined as follows:

require(<condition to be validated> , <message to be displayed if the condition fails>);

assert(): The assert function, like require, is a convenience function that checks for conditions. If a condition fails, then the function execution is terminated with an error message.
assert() takes only one parameter as input. You pass a condition to assert(), and if the condition is true, then the function execution continues and the execution jumps to the next statement in the function. The assert() statement is defined as:

assert(<condition to be checked/validated>);

revert(): Can be used to flag an error and revert the current call. You can also provide a message containing details about the error, and the message will be passed back to the caller. However, the message, like in require(), is an optional parameter. revert() causes the EVM to revert all the changes made to the state, and things return to the initial state or the state before the function call was made.
The reason for reverting is that there is no safe way to continue execution because something unexpected happened. This is important as it helps in saving gas.

Since the function execution stops after the revert() statement, the remaining gas is also returned back to the user. If you don't use the revert() statement and some error occurs, then the entire gas is lost. Using revert() does not return the consumed gas, however. The gas that is consumed is consumed, and it cannot be returned.
## Getting Started
You Guys Can Practice Using Error Handlers in Solidity With The Help Of Basic Contract That I Provided With This Project This Contract "Error" Contain Test Functions for Testing Each Of The Error Handlers And Has A Brief Note About What Are Their Specifications Download The Contarct From The Repository

### Installing

* You Can Get acess To the Contract By Simply Going To The Repository File Section And Can Run In Any Online And Offline Enviornment 
* popular Offline IDE Such As Vscode Or ONline IDE Like Gitpod Or Remix Can Be Used!!! For This Project I Recommend To Use Remix As This Platform Is Dedicated To Run Solidity Program And Has Many Features No Need For Any Kind of Extensions!!

### Executing program

* Simply Import The Contract To Your IDE And Start Your Program By: 
* Compile The Contract
```
COMPILE
```
* Deploy The Contract
```
DEPLOY
```
*After You SucessFully Deployed Contract You Can Start Testing The Error Handlers By Giving Values(i) And Running The TestFunctions(TestRequire,TestAssert,TestRevert)
```
testrequire----->i=x------->run
```
*You Guys Can Change The Value Of 'num' And Can Test The Assert Also Can Change The Error Message And The Conditions For The Error Handlers To  Become TRUE!!! 
## Help

If You Guys Have Any Doubts Related To Error Handelers Or The Contract That I Give Feel Free To Ask  For that On My Gmail
```
iamoneofthechoosen1@gmail.com
```

## Authors

Contributors names and contact info

ex. Dabi 
ex. [@Dabi](iamoneofthechoosen1@gmail.com)


## License

This project is licensed under the [Dabi] License - see the LICENSE.md file for details
