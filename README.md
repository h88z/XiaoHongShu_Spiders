# 小红书爬虫
---
持续优化更新的小红书爬虫，目前短时间内暂不打算开源。有使用需求可扫码联系，欢迎厂商老板或有创业想法的朋友一起交流。
---

<img decoding="async" src="https://github.com/h88z/XiaoHongShu_Spiders/blob/main/wechat.jpg" width="30%">

---
功能介绍
---

1. 关键字爬取笔记及作者数据
   1. 笔记数据
      1. 笔记ID及链接
      2. 笔记类型(图文笔记或视频笔记)
      3. 笔记标题
      4. 笔记内容
      5. 笔记发布时间(年-月-日 时-分-秒)
      6. 点赞数
      7. 收藏数
      8. 评论数
      9. 分享数
   2. 作者数据
      1. 账号ID
      2. 账号昵称
      3. IP归属地(精确到市)
      4. 账号小红书等级
      5. 达人量级(素人、KOL、KOC、腰部、肩部、头部等)
      6. 粉丝数(精确到个位)
      7. 关注数(精确到个位)
      8. 被点赞总数(精确到个位)
      9. 被收藏总数(精确到个位)
      10. 发布笔记总数(精确到个位)
2. 生成统计exal表格
3. 根据表格内容某项生成类别统计饼状图

## 版本更新记录

### 即将实现
1. 进程通信，数据交互
2. 自动跳过已存笔记
3. 断点继续
4. 断网判断，刷新等待
5. 添加按条件筛选功能(按最新、最热、综合筛选/按图文、视频筛选)
6. 关键词强匹配
7. 生成的表格名及工作簿按需求命名

---
2023-09-07(V1.0)
---

### 待优化
1. 偶尔会在每页最后一个笔记的时候（输出"本页第X个笔记"之后）找不到元素，需要再排查下，不影响功能但影响效率。
2. 备注的那段导致的问题。

### 已更新
1. 优化速度
2. 优化高度判断
3. 乱七八糟的问题若干(记不起来了)

## 其他备注
1. xhs 56-62行 这段功能当初为什么要加，现在看有点画蛇添足，感觉没什么意义，因为没时间不敢随便删。明天有空再看下，目前影响不大。
2. 爬一段时间后，再刷新会出现之前爬过的内容和新内容混杂的情况。暂不清楚什么原因，值得后续抽时间研究下。
