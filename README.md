# EasyGoSpider
### “宜出行”热力图数据爬虫: 	

-----

> 
1. 效果受制于部署账号数量，需自行到某宝购买  :pill:
2. yundama部分的代码没有上传，如有需要请自行搜索相关api

### 已完成：
* 部署多账号，自动登陆、识别验证码（手动识别或借助yumdama平台）、获取cookies
* 指定区域爬取（已测试全成都市范围30天稳定运行）
* 断点续爬
* 定时周期爬取（当前一个小时内的数据算一次任务，每两小时一次）

### 基于：
* python27
* scrapy
* mongodb

:)

-----

2017-10-18更新：

### 关于数据转换成经纬度：
这个问题我在知乎问过，得到的答案是这样的：
> `grid_x`通过公式`1e-6 * (250.0 * grid_x + 125.0)`转换成经度，纬度同理

因为我只需要爬数据，并没有去验证这个公式，欢迎反馈

现在看发现写得很烂，不要模仿，后面有机会优化一下= =
