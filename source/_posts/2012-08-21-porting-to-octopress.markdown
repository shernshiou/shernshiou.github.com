---
layout: post
title: "Porting to Octopress"
date: 2012-08-21 11:39
comments: true
categories: [Life, Blog]
---
I have slowed down my updates on my blog these months. Lately, I spend my time travelling so do my works. The other reason behind the reduced of new posts because I am considering alternative platform to Posterous. Some of you might know that Posterous is winding down after the acquisition by Twitter. After several trials, I've decided to settle with Octopress hosted with Heroku due to several reasons:-

1. Complete mirror of local copy
2. Changes are tracked with Git
3. Markdown
4. Code snippet with Pygments (find some of them at [Code Categories](/blog/categories/code/))
5. Awesome mobile theme

But this platform has several downside compared to Posterous

1. Lack of other ways of posting (e.g. email, mobile)
2. Hard to embed without writing some changes
3. I'm not familiar with Ruby
4. Size matters at Heroku (for free hosting)

I'm at about 80% of the total progress because I am still finding ways to include more images (by including other hosting) and porting embedded IFrame. One custom changes I've made on this blog is the ability to display LaTeX Math Equation with Kramdown (thanks to [Greglus](http://greglus.com/blog/2011/11/29/integrate-MathJax-LaTeX-and-MathML-Markup-in-Octopress/)). 