# 5-topics

# Task 1
## WHAT ARE 5 TOPICS WE'VE COVERED THUS FAR?

## 1. Mocha
npm install -g mocha

## 2. PORT
const PORT = process.env.PORT || 8000;

## 3. Fetch
const fetch = require('node-fetch');

fetch('https://api.spacexdata.com/v3/capsules')
.then(response => {
    console.log(response);
    return response.json();
})
.then(data => {
    console.log(data);
})

## 4. Express
const express = require('express');
const app = express();

## 5. Axios
const axios = require('axios');

# Task 2
## TAKE ONE OF YOUR ENGINEER CLASSMATES' DESCRIPTION AND EXAMPLE OF EACH TOPIC AND ADD ON

# week4recap #
## AJAX - Asynchronous Javascript and XML ##
- Ajax allows users on webpages to interact with servers through HTTP (protocol) -> Made even better with the Fetch API.
- Async/ await functions
```
async function getUserData() { 
    const url =  'https://google.com/gmail/users'; 
    let users = await fetch (url).then(res => res.json()); console.log(users); }
```
## FETCH ##
- make API requests using javascript -> get Data
```
fetch(requestURL)
     .then(function(responseData){
         return responseData.json();
     })
     .then(function(jsonData){

     })
```
## SQL ##
- Personal Favorite
- Store and access data efficiently in ~databases~
- Allows us to create and query for specific data
```
SELECT name, age FROM teachers;
```
## AJAX IN JQUERY ##
$.get() and $.post()
```
$.get('https://www.reddit.com/bio', {
    q: 'birthdays'
}).done(function(data) {
    console.log(data);
});
```
## PROMISES ##
- Because async functions can not run at the same time
- Makes promise to run before or later
```
$.get('https://www.google.com/fellofftherocks').done(function(data {

}).fail(function(error) {

}));