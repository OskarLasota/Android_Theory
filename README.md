# Android Theory

## Interview Questions

### 1) Can you tell me why you don’t want memory leaks in your app ?

Memory leaks occur when the garbage collector is not able to clear unused objects which means that they will be stored in the ram until the application is closed.This can lead to performance issues or worse, to OutOfMemoryError crashes. A good example of a memory leak could be using Singletons, as you probably know, singletons are initialized once and survive the entire application lifecycle, passing an activity context into a singleton means that the reference of activity will remain even when the activity is no longer in use. This will put unnecessary strain on the RAM. This example could be avoided by passing on the application context instead.

### 2) Can you explain how you would pass on data from a fragment to an activity ?


### 3) What is the difference between unit and integration testing? 

### 4) What is A/B testing?

### 5) What to consider when choosing between ListView and RecyclerView
I would use a ListView when the data that I want to display isn't dynamic. RecyclerView has much more power when it comes to displaying complex views or dynamic data. RecyclerView needs an adapter implementation where we are able to "recycle" the view once they get out of scope as well as it avoids the CPU-intensive process of loading the entire dataset at once, it will only load the amount of data that can be seen on the screen, unlike ListView which loads the entire data set.

### 6) What can you tell me about the ViewHolder pattern?

The ViewHolder pattern is used in the RecyclerView Adapter and allows us to scroll through the list smoothly as it stores row view references hence leading the findViewById function only once on binding. 

### 7) What can you tell me about the LayoutManager?

The LayoutManager takes responsibility for laying out row views and allows us to choose the way we want to display our data, whether we want to display data in a linear layout or grid layout and if so, how many data points per row. We can also set the orientation of the scrolling of the data set.


