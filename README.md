# Motivation

This Tampermoney script aims to make articles published on Wechat more readable
on desktop screens, which usually have more width than height.

The default layout of Wechat article is clearly in favour of mobile phones, which
are held in hands and have more height than width.

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