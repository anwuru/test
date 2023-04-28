---
layout: post
title: 解决 OOM 
categories: [Java]
description: 经过排查最终解决。
keywords: Error, OOM
---



### 

控制台打印：

```
……
[Loaded Script1 from file:/groovy/shell]
a = 9, result is false
[Loaded Script1 from file:/groovy/shell]
a = 3, result is true
[Loaded Script1 from file:/groovy/shell]
a = 7, result is false
[Loaded Script1 from file:/groovy/shell]
a = 7, result is false
[GC (Metadata GC Threshold)  722452K->251702K(1090560K), 0.0483118 secs]
[Full GC (Metadata GC Threshold)  251702K->240778K(1254912K), 0.4303570 secs]
[GC (Last ditch collection)  240778K->241270K(1373696K), 0.0274501 secs]
[Full GC (Last ditch collection) 
[Unloading class Script1 0x00000007c103c428]
[Unloading class Script1 0x00000007c103bc28]
[Unloading class Script1 0x00000007c103b428]
[Unloading class Script1 0x00000007c103ac28]
[Unloading class Script1 0x00000007c103a428]
……
```

