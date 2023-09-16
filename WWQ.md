# Challenge Description:
Given a website where we have to answer a no. of questions to get to the flag.
# Approach:
## Question 1: Have you visited the /welcome endpoint?

We can visit the /welcome endpoint by adding '/welcome' to the url.

Welcome is the endpoint we have to visit.

This leads to a page with Answer 1: _Answer-1: This page doesn't exist._

## Question 2: Ever heard of http request/response headers visit /header enpoint to find out.

Appending /header to the url we get a page that tells us "There is something here"

Inspecting the page and going to the network tab after reloading the page we check out the 'header' file.

Checking the response headers tab we find _Answer 2: Intro to headers_
## Question 3: Browsers can store data too, checkout what are localstorages to find out
Inspecting the page and checking out the local storage under the storage tab gives us the answer for the third question.


## Question 4: Read about Document Object Model, i've hidden your answer somewhere here...
Inspecting the page we see answer 4 in a comment under the inspector tab.
_Answer-4: Did you read about the DOM?_
## Question 5: Often there is an endpoint called robots.txt, find out what it does..
We need to access the /robots.txt endpoint

robots.txt tells the search engine which urls aren't meant to be accessed
## Question 6: Learn about request methods, and answer what method is being used when you connected to this site?
_Answer-5: GET_
## Question 7: Here cookies are not what you think, Find out what cookies are, find some here too 
Inspecting the page we find the flag in a cookie value under the storage tab.

_Answer-6: You found the cookies_
# Flag Found
flag{H8dAL+eHPgPq1xGD7W/Euw==}
