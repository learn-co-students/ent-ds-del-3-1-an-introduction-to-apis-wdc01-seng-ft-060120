
# An Introduction to APIs


## Introduction
API's (Application Programming Interfaces) are proliferating, and they can make it much easier to automate the retrieval of information. In this lesson we'll provide an introduction to APIs so you have an idea of what they are, and why you might want to use them to access data.


## Objectives
You will be able to:
* Explain what an API is and why you might want to use one
* Explain the key limitations you need to look out for when working with a new API

## Easy, Automatic Access

Lets say an organization has information, is willing to share it, and you want a copy. Maybe it's a state that wants people to be able to get information on all business entities registered there. Maybe it's a government agency that wants to provide information on how well they're providing a given service. Once they've decided they want to share the information and you've decided you want it, what's the best way to make that happen?

Many years ago, you might have had to phone up the main number for the organization, get put through to someone on their IT team and ask if they could send you a file. It might have worked, but wasn't super efficient, easy or scalable.

Twenty years ago as the internet started to become more mainstream, the obvious solution was to put the information up on a website - something we'll be looking into next week when we tackle web scraping (writing scripts to automate the downloading of information from web pages). Some of the information got put up as web pages, some just got linked to, allowing you to download a csv file or something similar.

But at the same time, companies also started to offer access to their information (or services) through APIs.

If a web page is designed for a computer to share information with a ***person*** (the web server shares the information with the person browsing the website), an API is designed for a computer to share information with **another computer**. Web pages are optimized for being readable by humans *(or at least, they're supposed to be!)*. **APIs are optimized to make it easy for you to write a script so that your computer can go talk to their computer to get the information you need. **


## The Many Use Cases for APIs
APIs can actually be used for many things - not just for retrieving information. Twilio has an API that allows you to write a script to call their API to send text messages to people. GitHub has an API for creating new repositories. Many services have an API allowing a computer to automate a task that a person might otherwise have to do through a website - whether uploading a photo to Flickr, searching for a company name in a state database or getting a list of garbage collection times for a municipality.


## Limitations of APIs
When working with APIs, there are some limitations you have to be aware of - especially relating to scope and scale.
* **Scope** - Just because a company has an API and has information, it doesn't mean you can get all of the information through their API. Any time you want to get information from a given API, write a small test script and make sure it actually allows you to access the things you need in the way you require.
* **Scale** - Some APIs are provided for free as a public service. Others you have to pay for, or allow you to perform activities (like sending a text message) that you pay for. Whatever the commercial model, all APIs have some kind of rate limiting. Because it costs money to keep computers running and because you could write a script to ask lots and lots of questions of an API, generally an API will have some kind of limitations on the number of "API calls" you can make against the service per unit of time. Make sure that you know what the rate limits are and that your use case isn't going to need more API calls than you will be able to make.


## Summary

If there is an API to retrieve the information you want, it can be a very easy way to find and download that information. But make sure to test out the API to make sure it provides the information you need and look out for rate limits if you think you're going to have to make hundreds or thousands of API calls in a fairly short amount of time.


