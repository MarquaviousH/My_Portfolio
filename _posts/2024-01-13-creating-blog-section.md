---
layout: post
title:  "Website Dev log 1"
date: 2024-01-13 02:53:00 +0000
categories: blog
permalink: /web-dev-log1.html
---

Hello all, currently Im trying to figure out how to get my landing page working for my blogs. I want a page that will allow users "(like you)" to see all of my post that I have made for my blogs. The thing is the way I am currently set it up, it is acting up. The thing is about developing apps, websites, or programs, there will be a time when something doesn't go right like as plainned.

So the next best way is to trouble shoot on what is making this problem. A good way to trouble shoot problems is to have resoures on the language you are working with, documentation of what software you are using, and anything else that can help you trouble shoot your problem. For this entire website I used: Docker, HTML, CSS, and SCSS. Eventually, I will use Javascript to make the website have more functionity than being static.

To trouble shoot the problem I am having of setting up a landing page, I am using documentation for Jekyll. So the problem that I am having is that everytime you click on the link of a blog, it will say that "error page not found". I am trying to figure out why it is doing that even through the actually page for my blogs are made. The main thing is to keep trying as you are frustrated and look at your documentation. If you need to take a small break to refresh yourself then go ahead and take that break. But come back to tackle the problem.

<b>Update:</b>
I figure out the problem. The problem was with the URL. Ever since I started making the website, I have gotten problems linking the pages property together. So I did some research and I was able to find out that I need to use "| relative_url" in linking the urls. Check out these two pages helping to explain more about relative url and base url: <a href="https://jekyllrb.com/docs/liquid/filters/">Jekyll website.</a> and <a href="https://talk.jekyllrb.com/t/relative-url-and-baseurl/2051">Jekyll Discussion place.</a>

Basically how the relative url works is that it takes the url you made for a page then it will append it to the root of the website. So it will do the work of creating the whole url instead of you making the whole url for each page that you make. When I created the landing page, it list all the pages that are apart of the blog category. Everytime I press the link of the blog post, it will say that the page doesn't exist. The thing is that in my landing page I did not use the relative url and it will do my local host/example-of-website.html. It did not added to the end of the base url. but when using the relative url, it adds the webpage url to the end of the base url and connect directly to the webpage.