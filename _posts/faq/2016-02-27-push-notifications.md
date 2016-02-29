---
layout: post
title: Push Notifications
modified: 2016-02-27T12:12:04+11:00
categories: faq
excerpt: "How to setup push notifications"
tags: []
image:
  feature:
date: 2016-02-27T12:12:04+11:00
author: matt_delves
---

Push Notifications are unfortunately somewhat complex as they require you to configure a webhook in Buildkite that points to the boxkiteapp notifications server.

To have push notifications work, you need to configure the webhook to point to the URL https://notifications.boxkiteapp.com/receive

The webhook should use v3 of the Buildkite webhook which uses pipelines instead of projects.
