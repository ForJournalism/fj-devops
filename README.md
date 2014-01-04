# DevOps Course Outline

You have an app running locally that lets people explore data. Great. How will anyone find it, though?  You can't serve this off your laptop.

And if they do happen to find your app running on your laptop somehow, your localhost don't scale!

We'll also cover basic terminology and concepts.

## Definitions

* Devops
* Sysops
* Secops/infosec

## Version Control

See the GitHub for Journalism material.

## Tests & Continuous Integration

Are these topics going to be covered in each app-building course?

## Deployment

What does "deploying an app" mean? Explainer TK.

### Options

* capistrano (ruby)
* fab (python)
* rpm/deb

### Strategies

* Scheduled releases
* Continuous deployment

## Caching

* in memory
* persistent
* headers
* template or data fragments, entire pages

### Software

* [http](https://github.com/rtomayko/rack-cache)
* [memcached](http://memcached.org/)
* [redis](http://redis.io)
* [varnish](https://www.varnish-cache.org/)
* [nginx](http://nosql.mypopescu.com/post/17651985814/high-performance-rails-caching-with-redis-and-nginx)

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
  * in request like http headers
  * external like varnish
  * layers to cache on and what to cache at each

## Monitoring

Things you can monitor:

* system load/CPU/memory with things like monit, upstart
* services (nginx, MySQL, etc) again with monit, upstart or similar
* apps (memory usage, exceptions)
* response times (internal or external ways like pingdom)

## Scaling

  * manual vs auto
  * horizontal (throw more machines at it)
  * optimization
