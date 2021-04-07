# Android Theory

## Interview Questions

### 1) Can you tell me why you don’t want memory leaks in your app ?

Memory leaks occur when the garbage collector is not able to clear unused objects which means that they will be stored in the ram until the application is closed.This can lead to performance issues or worse, to OutOfMemoryError crashes. A good example of a memory leak could be using Singletons, as you probably know, singletons are initialized once and survive the entire application lifecycle, passing an activity context into a singleton means that the reference of activity will remain even when the activity is no longer in use. This will put unnecessary strain on the RAM. This example could be avoided by passing on the application context instead.

### 2) Can you explain how you would pass on data from a fragment to an activity ?


### 3) What is the difference between unit and integration testing? 

### 4) What is A/B testing?
