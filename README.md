
Alfred Workflow for bilibili.com
========================

本作是一个 [Alfred2](http://www.alfredapp.com/) 的工作流，用于搜索 [bilibili.com](http://bilibili.com) 上的视频内容。(也可用于 Alfred 3)

## 安装方法：

```shell
bash build.sh
open bilibili.alfredworkflow
```

## 使用方法：

打开 Alfred 后，输入关键字 **bilibili** 即可开始搜索，搜索分为2种模式。

### 关键词查询

输入 **bilibili 关键词** 即调用bilibili.com的查询接口，出于国内网络速度和B站服务器带宽的考虑，所以搜索可能较慢（还有因为解析裁减了图片），默认以 **综合** 进行排序。（后期不定时可能会改进，看心情）

与B站的搜索一样，你可以输入 **bilibili 冰果@动画** 来指定在某个频道下搜索。

![关键词查询](screen-capture/search-keywords.png)

### 频道查询

工作流内置了多个频道关键词，当畭 **bilibili 频道关键词** 时，会抓取该频道下的第一页的内容，如输入 **bilibili 新番** 会抓取[二次元新番](http://www.bilibili.com/video/bangumi-two-1.html)下的视频，在B站不调整的前提下，一页有24个视频，按审核通过时间倒序排列。

频道关键词列表如下：

- MAD: 动画 - MAD.AMV
- AMV: 动画 - MAD.AMV
- MAD.AMV: 动画 - MAD.AMV
- MMD: 动画 - MMD.3D
- MMD.3D: 动画 - MMD.3D
- 二次元鬼畜: 动画 - 二次元鬼畜
- 期刊: 动画 - 期刊.其它
- 音乐视频: 音乐 - 音乐视频
- 三次元音乐: 音乐 - 三次元音乐
- VOCALOID: 音乐 - VOCALOID相关
- VOCALOID相关: 音乐 - VOCALOID相关
- 翻唱: 音乐 - 翻唱
- 游戏视频: 游戏 - 游戏视频
- 游戏攻略: 游戏 - 游戏攻略.解说
- 游戏解说: 游戏 - 游戏攻略.解说
- MUGEN: 游戏 - MUGEN
- 科普知识: 科学技术 - 科普知识
- 人文地理: 科学技术 - 人文地理
- 全球科技: 科学技术 - 全球科技
- 野生技术: 科学技术 - 野生技术
- 生活娱乐: 娱乐 - 生活娱乐
- 舞蹈: 娱乐 - 舞蹈
- 三次元鬼畜: 娱乐 - 三次元鬼畜
- 影视: 娱乐 - 影视
- 新番: 新番 - 新番二次元
- 新番二次元: 新番 - 新番二次元
- 新番三次元: 新番 - 新番三次元

![频道查询](screen-capture/search-channel.png)

## 备注：

目前所有频道并未全部测试。

因为后续 B 站可能会更改页面结构，所以并不能保证本 Workflow 一直可用。