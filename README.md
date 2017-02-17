# Further Javascript - News App
### [Makers Academy] (http://www.makersacademy.com) - Week 7 Group Project

## Team Members
* [Matt Perry](https://github.com/thesedatedprince)
* [Rob Brentnall](https://github.com/treborb)
* [Adrian Eyre](https://github.com/adrianeyre)
* [James Turner](https://github.com/JamesTurnerGit)
* [Ben Carson](https://github.com/BenJohnCarson)
* [Joe Marriott](https://github.com/j-marriott)

## Index
* [Task] (#Task)
* [Technologies] (#Technologies)
* [Installation] (#Install)
* [User Stories] (#Stories)
* [Test Framework] (#Framework)

## <a name="Task">Task</a>
Single Page Notes App

This is a single-page notes app allowing users to view news headlines, and have it
appear in a list. News headlines can then be expanded to show the article.

We were asked to create a testing framework in Javascript from scratch. Once the framework had been completed we could then use it to test or applicaion.

## <a name="Technologies">Technologies</a>
* Javascript
* Node http-server
* HTML
* CSS
* [Waffle] (https://waffle.io/thesedatedprince/news-app)

## <a name="Stories">User Stories</a>
```
As a busy politician
I can see all of today's headlines in one place
So I know what the big stories of the day are

As a busy politician
I can read a summary of a news article
So I can get a few more details about an important story

As a busy politician
I can read a full news article
So that I can get an in depth understanding of a very important story

As a busy politician
I can see a picture to illustrate each news article when I browse headlines
So that I have something nice to look at

As a busy politician
I can read the site comfortably on my phone
Just in case my laptop breaks

As a busy politician
I can see whizzy animations in the app
To make my news reading more fun
```

## <a name="Install">Installation</a>
To use the news app and install node http server, follow these instructions:

```
$ git clone https://github.com/adrianeyre/news-app
$ cd news-app
$ npm install http-server -g
$ http-server
$ open -a safari localhost:8080
```

### News app screenshot
[![ScreenShot1](https://raw.githubusercontent.com/adrianeyre/news-app/master/images/screenshot1.png)](https://raw.githubusercontent.com/adrianeyre/news-app/master/images/screenshot1.png "Screen Shot 1")

## <a name="Framework">Testing Framework</a>
the repo includes a bespoke testing framework written from scratch.

### Installation
To install to any project
```
$ git clone https://github.com/adrianeyre/news-app
$ cd news-app
$ http-server
$ open -a safari localhost:8080/test.html
```

### usage

In order add additional tests to the app, please do the following:

```
1. Create a new test file in /spec, using JavaScript naming conventions.

2. Add this file to the head of test.html along with the file being tested.

3. Add your tests to your new spec file.

4. Open/refresh test.html in browser to see the outcome of these tests.
```

The testing framework follows these syntax conventions:

```
1. A describe block containing a description of the testing suite.

2. An it block describing the test to be run.
```

Example syntax of a simple describe/it block:
```js
describe("Test suite 1", function() {
  it('returns HELLO', function(){
    return assert.Equals(returnTrue(),true);
  });
});

```

### matchers
The following matchers are present in this testing framework:

```
Equals: Returns true if argument A is equal to argument B.
NotEquals: Returns true argument A is not equal to argument B.
GreaterThan: Returns true if argument A is greater than argument B.
LessThan: Returns true if argument A is less than argument B.
Contains: Returns true if argument A contains argument B.
HasContent: Returns true if argument A has content from argument B.
```

### custom fail messages
You can add a custom fail message by replacing argument C in the test:

```js
describe("Test suite 1", function() {
  it('returns HELLO', function(){
    return assert.Equals(returnTrue(),"HELLO", ":(");
  });
});
```

This will now return ":(" on fail.

### Test framework output

[![ScreenShot2](https://raw.githubusercontent.com/adrianeyre/news-app/master/images/screenshot2.png)](https://raw.githubusercontent.com/adrianeyre/news-app/master/images/screenshot2.png "Screen Shot 2")


