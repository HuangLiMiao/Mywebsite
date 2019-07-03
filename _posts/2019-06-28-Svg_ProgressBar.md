---
layout: page
excerpt_separator: "<!--more-->"
title: svg也可以成为进度条
categories:
  - svg制作
tags:
  - svg
---
#### 进度条例子

<hgroup class="circle-load">
    <svg width="240px" height="240px" version="1.1" xmlns="http://www.w3.org/2000/svg">
        <circle cx="110" cy="110" r="90" stroke-width="10" stroke="gainsboro" fill="none"></circle>
        <circle cx="110" cy="110" r="90" stroke-width="10" stroke="darkturquoise" fill="none" class="circle-load-svg"></circle>
    </svg>
</hgroup>
<style type="text/css">
.circle-load {
    position: absolute;
    width: 200px;
    height: 200px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.circle-load-svg {
    stroke-dasharray: 0 570;
    animation: rot 8s linear infinite;
}

@keyframes rot {
    100% {
        stroke-dasharray: 570 570;
    }
}
</style>

### 相关代码
```markdown
<hgroup class="circle-load">
    <svg width="240px" height="240px" version="1.1" xmlns="http://www.w3.org/2000/svg">
        <circle cx="110" cy="110" r="90" stroke-width="10" stroke="gainsboro" fill="none"></circle>
        <circle cx="110" cy="110" r="90" stroke-width="10" stroke="darkturquoise" fill="none" class="circle-load-svg"></circle>
    </svg>
</hgroup>
<style type="text/css">
.circle-load {
    position: absolute;
    width: 200px;
    height: 200px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.circle-load-svg {
    stroke-dasharray: 0 570;
    animation: rot 8s linear infinite;
}

@keyframes rot {
    100% {
        stroke-dasharray: 570 570;
    }
}
</style>
```
