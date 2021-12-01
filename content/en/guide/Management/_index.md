---
title: "Part 9: Project Management"
linkTitle: "Part 9: Project Management"
weight: 11
description: >
  Several means of team communication, source control, and planning have been adopted. They are mentioned here.
type: docs
---

## Source Control

1. Front end, including web pages served as static resources: https://github.com/Mashweb/web-call.cc
1. Back end: currently none. The web pages containing the front end code are simply served as static resources by a web server like Apache 2, Nginx, or Hunchentoot. At some point a Hunchentoot or Ruby on Rails backend will be put in place. It will provide authentication and authorisation for access to the back end database.
1. Back end database: a special purpose, Common Lisp based RESTful web service exists to serve HTML DOMs stored as s-expressions: https://github.com/Mashweb/ZenDatabase
1. Associated Ruby on Rails based "non technical" club website: https://github.com/Mashweb/mashweb.club
1. Static web pages served by GitHub Pages and accessed by the subdomain doc.mashweb.club, containing some demos and documentation (mostly the white paper): https://github.com/Mashweb/mashweb.github.io
1. WordPress pages on the subdomain blog.mashweb.club: accessed via a WordPress admin login.

## Team Discussions

See https://github.com/orgs/Mashweb/teams/pre-alpha-zen/ .

## web-call.cc Wiki

See https://github.com/Mashweb/web-call.cc/wiki .

## Agile Development Management\

See https://www.pivotaltracker.com/n/projects/70151

## Quick Sharing

Some facilities for quick sharing of demos and prototypes:
1. No-IP.com and alternatives (or go directly to a comparison of the top 5)
1. ngrok.com
