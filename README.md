Scalding Exercise 
====================

This is a simple exercise for Scalding Developers.
The purpose is to write a Scalding Job to analyse the content of the access logs generated by a web application. 
An example of those logs is in the file events.log in this directory.

## Input

Events are indicating the following information:

- timestamp: the time of the event expressed as epoch value 
- userId: the identifier of the user, extracted by the request headers
- action: the HTTP verb associated to the operation
- actionData: other information associated to the operation

The purpose is extract statistics about the number of sessions per users. In more detail we want to extract:

- The average session duration 
- The average number of actions per session. 

A user session is defined by a series of user actions separated by an interval of time less than 10 minutes

## Required Output

Home exercise: 

A Scalding Job class plus its runner and all the tests required to prove that the implemented logic works.

Shorter face to face interview: 

the main logic of the scalding job. A description of the main macro-functions to implement and an implementation of at least one of them. The 