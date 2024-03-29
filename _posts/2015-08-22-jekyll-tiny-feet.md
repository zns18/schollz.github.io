---
layout: post
title: Tiny Feet - a super minified fully-featured Jekyll blog
date: 2015-08-19
comments: true
archive: false
tags: [web development, blogging, jekyll]
landing: true
description: Trying to make a tiny footprint version of a nice blog website
---

Typical mobile-friendly pages call for special CSS to handle the different viewing sizes. Often this comes in the form of Bootstrap, and then add-ons with Font Awesome and JQuery to make it look extra nice. Here's a breakdown you might expect from a typical website:

Includes | Compressed | Size
--- | --- | ---
Content HTML | 10 KB | 10 KB
Font Awesome | 7 KB | 30 KB
Bootstrap CSS + JS | 35 KB | 156 KB
JQuery | 33 KB | 94 KB
Google Analytics | 11 KB | 25 KB
Disqus | 22 KB | 64 KB
Total | 118 KB | 379 KB

The content HTML of the site is less than a tenth the actual bandwidth used to transfer it, for a typical site. Of course, connections are faster than ever (and cheaper too), so this shouldn't really matter. You have me there. However, I like the principle that when information is transfered, the information is utilized. When I have used all the fancy mobile stuff, I found that I wasn't using most of it.

This prompted me to create a new theme that does the major things (navigation, nice font awesome-like icons, searching, mobile-friendly) without all the bloat from the major HTML packages. My solution is the [Tiny Feet theme for Jekyll](https://github.com/schollz/jekyll-tinyfeet).

Creating my own theme with my own custom CSS reduced the landing page to only 8 KB compressed (24 KB uncompressed), **total**! Here are some details of the theme:

<h2><svg version="1.2" baseProfile="tiny" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
	 x="0px" y="0px" width="40px" height="40px" viewBox="-19.9 821.4 40 40" xml:space="preserve">
<g>
	<path fill="#010002" d="M11.1,827.9c-2.9-1-5.8,0.9-6.7,3.7c-1,3.1,0.6,7-0.1,8.9c-1,2.7-3.9,6.8,0.1,9.6c3.6,2.5,6.3-1.5,8.2-5
		c1.5-2.7,3-5.5,3.6-8.4C16.6,834.4,16.8,829.9,11.1,827.9z"/>
	<path fill="#010002" d="M5.6,828.1c1.4,0,1.9-1.3,1.9-2.8c0-1.6-1.1-2.8-2.5-2.8c-1.4,0-2.5,1.3-2.5,2.8
		C2.4,826.8,4.2,828.1,5.6,828.1z"/>
	<path fill="#010002" d="M10.1,826.9c1.2,0,2.1-1.9,2.1-3.4c0-1.5-0.9-2.1-2.1-2.1c-1.2,0-2.1,0.6-2.1,2.1
		C8,825,8.9,826.9,10.1,826.9z"/>
	<path fill="#010002" d="M16,826.7c0.7-0.9,0.3-1.9-0.4-2.6c-0.7-0.7-1.6-0.9-2.2,0c-0.7,0.9-0.9,2.7-0.1,3.4
		C13.9,828.3,15.3,827.7,16,826.7z"/>
	<path fill="#010002" d="M18.5,827.4c-0.6-0.8-1.3-1.1-2.1-0.3c-0.7,0.8-1.1,2.3-0.5,3.1c0.6,0.8,2,0.4,2.7-0.3
		C19.3,829.1,19.1,828.2,18.5,827.4z"/>
	<path fill="#010002" d="M20,831.9c-0.2-0.8-0.7-1.3-1.4-1c-0.7,0.3-1.5,1.3-1.2,2c0.2,0.8,1.3,1.1,2,0.8
		C20.1,833.4,20.2,832.7,20,831.9z"/>
	<path fill="#010002" d="M-4.1,842.2c-1-2.8-3.8-4.7-6.7-3.7c-5.7,1.9-5.5,6.5-5,8.8c0.6,2.9,2.1,5.7,3.6,8.4c1.9,3.6,4.5,7.6,8.2,5
		c3.9-2.7,1.1-6.9,0.1-9.6C-4.8,849.2-3.1,845.2-4.1,842.2z"/>
	<path fill="#010002" d="M-4.6,833c-1.4,0-2.5,1.3-2.5,2.8s0.5,2.8,1.9,2.8c1.4,0,3.2-1.3,3.2-2.8C-2.1,834.2-3.2,833-4.6,833z"/>
	<path fill="#010002" d="M-9.8,837.4c1.2,0,2.1-1.9,2.1-3.4c0-1.5-0.9-2.1-2.1-2.1c-1.2,0-2.1,0.6-2.1,2.1
		C-11.9,835.5-11,837.4-9.8,837.4z"/>
	<path fill="#010002" d="M-12.9,838.1c0.7-0.7,0.5-2.4-0.1-3.4c-0.7-0.9-1.5-0.7-2.2,0c-0.7,0.7-1.1,1.6-0.4,2.6
		C-15.1,838.2-13.7,838.8-12.9,838.1z"/>
	<path fill="#010002" d="M-16.2,837.6c-0.7-0.8-1.5-0.4-2.1,0.3c-0.6,0.8-0.8,1.7-0.1,2.4c0.7,0.8,2.1,1.1,2.7,0.3
		C-15.1,840-15.5,838.4-16.2,837.6z"/>
	<path fill="#010002" d="M-18.4,841.4c-0.7-0.3-1.2,0.2-1.4,1c-0.2,0.8-0.1,1.5,0.6,1.8c0.7,0.3,1.8,0,2-0.8
		C-16.9,842.7-17.6,841.7-18.4,841.4z"/>
</g>
</svg>&nbsp; Jekyll Tiny Feet theme</h2>

- Very small footprint for landing page (CSS+JS < 10 KB uncompressed)
- SVG Icons for fast loading (< 4 KB uncompressed)
- Dynamic description loading on main page
- Fixed navbar
- SEO and Opengraph
- Tag page and tags underneath each post title
- Optional Disqus comments on posts
- Optional Google analytics


## Acknowledgements

- [Jekyll for base theme](https://github.com/jglovier/jekyll-new)
- [christian-fei for simple-jekyll-search](https://github.com/christian-fei/Simple-Jekyll-Search)
- [nadjetey for gist idea](https://github.com/nadjetey/wangana)



