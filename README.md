# DevOps Course Outline

## Introduction

You have an app running locally that lets people explore data. Great. How will anyone find it, though?  You can't serve this off your laptop.

And if they do happen to find your app running on your laptop somehow, your localhost don't scale!

We'll also cover basic terminology and concepts.

## Definitions

* Devops
* Sysops
* Secops/infosec

## Responsibilities, tools and analytics

* Typical day
* Launch day
* Doomsday

## Intro to command line

## Version Control

See the GitHub for Journalism material.

## Testing and Continuous integration (TravisCI, CircleCI)

## Error logging (?OSS, Sentry)

## Performance (Graphite, NewRelic)

## Deployment

* What does "deploying an app" mean? Explainer TK.
* Intro to VirtualBox, vagrant, docker, salt and other provisioning tools:
* How they work together
* What to use and why

## Basic projects
* Host static site on GitHub
* Host static site on S3
* Local env setup with Vagrant for one lang
* Single-server Heroku hello worlds for Node, Sinatra, Rails, Flask, Django, Clojure
* Single server Heroku with databases of your choosing

## Strategy and Project Managmeent

* Scheduled releases
* Continuous deployment

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

## Caching

* in memory
* persistent
* headers
* template or data fragments, entire pages

### persistent

* database / inc redis
* filesystem

### invalidation

* 2 hard problems
* busting
* w/o causing pile up

### some of the many levels

* local
* in app
* in request like http headers
* external like varnish
* layers to cache on and what to cache at each

### Software

* [http](https://github.com/rtomayko/rack-cache)
* [memcached](http://memcached.org/)
* [redis](http://redis.io)
* [varnish](https://www.varnish-cache.org/)
* [nginx](http://nosql.mypopescu.com/post/17651985814/high-performance-rails-caching-with-redis-and-nginx)

## Intermediate projects

* Deploy PANDA on EC2
* Two-server Heroku with manual deployments and data migrations
* Two-server Heroku with CI from master and stable branches
* Add caching and CDN
* Deploy app on VPS via Salt+Docker

## Case studies

* Election 2012
* Sochi 2014
* SEA

# Advanced project:
? Walk through an active deployment to look at logs and analytics then create new stack and move app ?
