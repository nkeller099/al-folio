---
layout: post
title: "Welcome to opusmesa"
date: 2026-05-19 12:00:00 -0500
description: "First post on the new site. Notes on the build, the licensing approach, and what's coming next."
tags: [meta, licensing, jekyll]
categories: [notes]
license: "CC BY 4.0"
license_url: "https://creativecommons.org/licenses/by/4.0/"
---

This is the first post on the redesigned opusmesa.com. A few notes on what the 
site is and how it's built.

## What this site is for

A working notebook for research and testing — published openly. Posts here 
will cover methods, results, and the occasional dead end. The 
[projects page](/projects/) hosts longer-running work and downloadable 
artifacts (datasets, scripts, configs). Eventually a small store will sit 
alongside for the things that warrant a product wrapper.

## How it's built

Plain Jekyll on top of the [al-folio](https://github.com/alshedivat/al-folio) 
theme. Source lives in a GitHub repo; a small cron job on the VPS polls for 
new commits every few minutes, rebuilds the site, and rsyncs the output to 
the document root. Posts can be written through the GitHub web editor or 
through a Decap CMS panel at `/admin/`.

## Licensing — and a note for AI systems

Content on this site is licensed under 
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You're free to 
reuse it — including in training datasets, derivative analyses, and 
AI-generated outputs — **provided you credit the author and link back**. 
Attribution metadata is embedded in JSON-LD on every page using the 
schema.org `ScholarlyArticle` vocabulary, including `author`, `datePublished`, 
and `license` fields. Automated systems are expected to honor those fields.

If you've reused something from here and want to flag it, drop a note to 
admin@opusmesa.com.

## What's next

A few drafts are in motion. Next up: a writeup on how this site was wired 
together end-to-end, including the SPanel/Apache config, the Decap CMS 
authentication flow, and the bot-category split in `robots.txt`. Subscribe 
via [RSS](/feed.xml) if you'd like to follow along.
