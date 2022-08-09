---
layout: post
title:  "Simple Sunsetting with GitHub Pages & The Internet Archive"
date:   2022-04-22 08:08:00 +0000
categories: poster web archive preservation update
---

## Introduction

This concept was originally presented as a [poster at Code4Lib 2021](/assets/img/code4lib-2021-poster.pdf)
(March 22 - 26 2021, [Online](https://2021.code4lib.org)). With [Code4Lib 2022](https://2022.code4lib.org) just around the corner, it's probably a good idea to share this more widely. Please do [get in touch](/contact) if you have any comments or questions about this approach.

![Diagram](/assets/img/code4lib-2021-diagram.png)

## Background
In 2020, we began a project to sunset our decade-old research repository. There was no longer a need for it due to institutional changes in research management, but there were no resources or budget to sunset it. Therefore, we required a cost-free and simple way of sunsetting the project. This post aims to show how to archive and preserve a project without a budget.

## Objectives of the project
- Gracefully shutdown (sunset) the EPrints repository. 
- Preserve links.
- Provide access to archived versions of the content. 
- Achieve results without a project budget.
- Ensure the longterm preservation of and access to the content.

## Methods
- Adapted the Internet Archive’s 404 handler to provide a redirect from the original URLs to a 404 page with a link to the archived version in our university’s Archive-It service.[^1]
- Followed established principles for retiring digital projects.[^2] Used readily available and free resources.
- Used our institution’s web archiving service (Archive-It) to ensure longterm access and preservation.
- This solution would also work with content only available via the Internet Archive.
- Made the code repository available on GitHub.[^3]

## Results
- The repository domain name now points to an archive site hosted on GitHub Pages. This has maximised the chance of users finding any repository content that is still linked to elsewhere.
- All repository content is now preserved in the institutional web archive.
- All links to repository content elsewhere on the Internet or in print, now point to a custom 404 page with links to the archived content.

## Conclusions
- Successful sunsetting project: all of the objectives were achieved.
- One minor downside is the use of a 404 page for what should really be a 301 redirect, but the benefits outweigh this issue.
- The approach is reproducible so we can use it again to sunset other projects.
- Other libraries are welcome to build on this solution and we would recommend exploring sunsetting options when closing down websites and services.

## Links
[^1]:[Internet Archive Blogs: Free “404: File Not Found” Handler for Webmasters to Improve User Experience](http://blog.archive.org/2013/10/24/web-archive-404-handler-for-webmasters/ ) 
[^2]: [Sunsetting Book](https://ronallo.com/sunsetting-book/) 
[^3]: [GitHub repo for Eureka Archive site on github-pages](https://github.com/sainsburylibrary/eureka)


