# mass-data-problem

## 后端响应巨量数据问题

首先考虑处理问题的方向：
1. 网络方向
2. 渲染方向

针对网络的问题，可以考虑：
- 与后端协商改接口规范，少给点数据
- 使用fetch stream方案流式获取数据
- 使用sse方案
- websocket

针对渲染性能的问题，可以考虑：
- 数据分页(需要先询问产品的意见)
- 分片渲染(比如React 底层渲染的机制类似的效果)
- 虚拟滚动(虚拟列表)
- 使用canvas去绘制数据展示
