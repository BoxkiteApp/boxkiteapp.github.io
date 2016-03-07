---
layout: post
title: Login With API Key
modified:
categories: faq
excerpt: "What are the scopes required for the Buildkite API key"
tags: []
image:
  feature:
date: 2016-02-27T12:18:17+11:00
author: matt_delves
---

At present to use Boxkite you need to provide a Buildkite api key that is configured with the following scopes:

* Read Organizations
* Read Agents
* Read User
* Read Builds
* Modify Builds
* Read Build Logs
* Read Pipelines

The only write access required is for builds as this allows you to rebuild, cancel and unblock a build from within the app.
