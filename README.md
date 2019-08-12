# Motivation

This Tampermonkey script aims to make articles published on Wechat more readable
on desktop screens, which usually have more width than height.

The default layout of Wechat article is clearly in favour of mobile phones, which
are held in hands and have more height than width.

# Installation

It has been published and synced to [GreasyFork](https://greasyfork.org/en/scripts/388428-%E5%BE%AE%E4%BF%A1%E6%96%87%E7%AB%A0%E6%A1%8C%E9%9D%A2%E6%8E%92%E7%89%88-wechat-article-desktop-layout).
Check it out!


# How to Use It

The default configuration will set the `max-width` to 1200px.
If fitting the screen width is desired, modify the code
```javascript
set_max_width("1200px");
```
to
```javascript
set_max_width("none");
```

# Mitigate the Side Effect

When the element of the article body is freed from `max-width = 677px`,
the QR code might obstruct it.
A simple fix of hidding the QR code element is then applied to mitigate this.
