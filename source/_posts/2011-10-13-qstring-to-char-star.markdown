---
layout: post
title: "QString to Char*"
date: 2011-10-13 00:00
comments: true
categories: [App, Code]
---
Thanks to [Qt Forum](http://developer.qt.nokia.com/faq/answer/how_can_i_convert_a_qstring_to_char_and_vice_versa)

Below help us to get Char* out from QString and the other way around:

``` c++ Convert QString to Char*
QString inputString = "hello";
QByteArray byteArray = inputString.toUtf8();
const char* cString = byteArray.constData();
```

``` c++ Convert Char* to QString
QString qString2 = QString::fromUtf8(cString);
```