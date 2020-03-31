# 加载

<!-- toc -->

## 异步加载js的方法

- defer：只支持IE如果您的脚本不会改变文档的内容，可将 defer 属性加入到`<script>`标签中，以便加快处理文档的速度。因为浏览器知道它将能够安全地读取文档的剩余部分而不用执行脚本，它将推迟对脚本的解释，直到文档已经显示给用户为止。

- async：HTML5 属性，仅适用于外部脚本；并且如果在IE中，同时存在defer和async，那么defer的优先级比较高；脚本将在页面完成时执行。

## 图片的懒加载和预加载

- 预加载：提前加载图片，当用户需要查看时可直接从本地缓存中渲染。
- 懒加载：懒加载的主要目的是作为服务器前端的优化，减少请求数或延迟请求数。

两种技术的本质：两者的行为是相反的，一个是提前加载，一个是迟缓甚至不加载。
懒加载对服务器前端有一定的缓解压力作用，预加载则会增加服务器前端压力。