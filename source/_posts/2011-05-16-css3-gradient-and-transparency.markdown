---
layout: post
title: "CSS3 Gradient and Transparency"
date: 2011-05-16 00:00
comments: true
categories: [Web, Code]
---
Due to inconsistency of CSS3 implementation across different web browser, I wish to leave some note on Gradient and Transparency.

#### Transparency
``` css Mozilla and Webkit based
background: rgba(0,0,0,0.3);
```
``` css IE based
background:transparent;
filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#50000000,endColorstr=#50000000);
```

#### Gradient
``` css Mozilla based
background: -moz-linear-gradient(rgba(255,131,126,1) 0%, (255,131,126,0) 95%;
```
``` css Webkit based
background: -webkit-gradient(linear, left top, left bottom, 
from(rgba(255,131,126,1)),to(rgba(255,131,126,0)));
```
``` css IE based
background:transparent;
filter: progid:DXImageTransform.Microsoft.gradient(startColorstr=#FFFF837E, endColorstr=#00FF837E);
```

### References:
1. MSDN [http://msdn.microsoft.com/en-us/library/ms532930.aspx](http://msdn.microsoft.com/en-us/library/ms532930.aspx)
2. Stackoverflow [http://stackoverflow.com/questions/2293910/css3-transparency-gradient](http://stackoverflow.com/questions/2293910/css3-transparency-gradient)
3. CSS Tricks [http://css-tricks.com/rgba-browser-support/](http://css-tricks.com/rgba-browser-support/)