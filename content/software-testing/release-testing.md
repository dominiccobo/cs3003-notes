---
title: "Release Testing"
date: 2020-01-16T12:35:30Z
---

## Release Testing Techniques

Software testing doesn't stop when creating the software. The more eyes we have on our software the more likely we are to expose defects, making releasing software in a controlled manner an important part of testing. There are several different techniques.

### Smoke Testing

How do we ensure the vital features of the application are working when it is released?

How do we know when the application is starting to burn? When an electronic appliance goes wrong, smoke is generally a good indicator of something bad. 

We aim to mimic this in Software Engineering by testing a piece of Software for its vitals.

### Alpha-Beta Testing

### A/B Releases

Most of what companies do when they want to deliver a new product is theorising over what a consumer may want. Often, they may deliver samples to a market and measure which one performs better.

In SE, this is known as A/B testing.

### Canary Releases

When mining was rife in the world, a canary used to be taken down into the mines to check for issues with air quality. The small lungs of the bird would mean it would be the first fatality in the event of a problem. Miners understood that when they no longer heard any chirping, they had to get out.

Learning from this, we can release a small piece of Software to customers to see whether it survives or dies. 

### Blue Green Releases

Is a technique of keeping a new version of an application running next to the old one, but using routing techniques to point the consumer to the new application when it is ready. 

That way if the new application isn't quite ready or fails, the routes can simply be changed back to the old application.


### Notes on Environments

Development

Staging

Production

