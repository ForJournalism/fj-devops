# DevOps Course Outline

----------------------

You have an app running locally that lets people explore data. Great. How will anyone find it, though?  You can't serve this off your laptop.

And if they do happen to find your app running on your laptop somehow, your localhost don't scale!

 You need to deploy it! But first, a quick word on... 

## Version Control

Or will this be covered in each app-building course?

And...

## Tests & Continuous Integration

Ditto this topic.

## Deployment

What is it?
  * Explainer

What are my options?
  * capistrano / ruby
  * fab / python

How often?

  * Scheduled releases
  * Continuous deployment

## caching
* in memory
  * framework
  * memcached
  * redis
  * varnish

* persistent
  * database / inc redis
  * filesystem

* invalidation
  * 2 hard problems
  * busting
  * w/o causing pile up

* some of the many levels
  * local
  * in app
  * layers to cache on and what to cache at each

## monitoring
  * system (load, CPU, memory)
  * service (nginx, MySQL, etc)
  * app
  * external (pingdom, etc)

## scaling
  * manual, horizontal
  * auto, ec2
