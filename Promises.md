#Promises
=========

http://www.html5rocks.com/en/tutorials/es6/promises/#toc-async

At their most basic, promises are a bit like event listeners except:

A promise can only succeed or fail once. It cannot succeed or fail twice, neither can it switch from success to failure or vice versa
If a promise has succeeded or failed and you later add a success/failure callback, the correct callback will be called, even though the event took place earlier
This is extremely useful for async success/failure, because you're less interested in the exact time something became available, and more interested in reacting to the outcome.

A promise can be:

fulfilled The action relating to the promise succeeded rejected The action relating to the promise failed pending Hasn't fulfilled or rejected yet settled Has fulfilled or rejected

Although promise implementations follow a standardised behaviour, their overall APIs differ. JavaScript promises are similar in API to RSVP.js. Here's how you create a promise:

    var promise = new Promise(function(resolve, reject) {
      // do a thing, possibly async, then…
    
      if (/* everything turned out fine */) {
        resolve("Stuff worked!");
      }
      else {
        reject(Error("It broke"));
      }
    });    
    
---
##Additional Links
https://github.com/domenic/promises-unwrapping/blob/master/docs/states-and-fates.md
