# lightData
有关知识图谱与自然语言处理的数据集，供自己研究学习实验，以及研究者、爱好者、工作者使用。

## 声明

本仓库的数据仅作为各高校或个人研究学习使用，如用于商业用途造成侵权等行为本人概不负责。

## corpus

### 1.百度百科图谱

目前提供两种类型的资源：词条数据信息，以及词条链接信息。

当前仅爬取少量数据，分别包含`1~10000`、`10000~90000`、`100000~1000000`个词条，使用者可自行拼接组合。

[网盘链接](https://pan.baidu.com/s/1nTeHYoc-NPR__TzJ6EekCA)，提取码：`jrrc`

#### 词条数据信息(baike_info)

如词条`霍克对空导弹`，[百科详情页](https://baike.baidu.com/item/%E9%9C%8D%E5%85%8B%E5%AF%B9%E7%A9%BA%E5%AF%BC%E5%BC%B9/1775036)如下图所示：

![UTOOLS1580436415757.png](https://lightsmile-img.oss-cn-beijing.aliyuncs.com/UTOOLS1580436415757.png)

爬取结果如下：

```json
{"info": {"word": "霍克对空导弹", "basic": {"title": "霍克对空导弹", "description": "霍克地空导弹系统是美国最老的防空导弹系统之一，自60年代初以来，一直是美国海军陆战队的主要防空武器。40年来，雷声公司总共制造了37000枚霍克导弹，每枚导弹的单位研制费为25万美元，每个火力单元（发射排）的单位换装费是1500万美元。霍克最初命名为“猛禽”，后来变成“全程寻的杀伤器”（HomingAlltheWayKiller）的缩写，即霍克。"}, "attrs": {"中文名": "霍克对空导弹", "外文名": "HomingAlltheWayKiller", "别称": "猛禽", "缩写": "霍克"}, "tags": []}, "type": "signal"}
```

其中`type`表示页面情况，有`none`,`signal`,`ambiguous`,`multiple`四种情况，分别表示无此条目，为单义条目，歧义条目，多义条目，具体信息可自行试验查看。

#### 词条链接信息(baike_href)

如词条`山东大学信息科学与工程学院`，[百科详情页](https://baike.baidu.com/item/%E5%B1%B1%E4%B8%9C%E5%A4%A7%E5%AD%A6%E4%BF%A1%E6%81%AF%E7%A7%91%E5%AD%A6%E4%B8%8E%E5%B7%A5%E7%A8%8B%E5%AD%A6%E9%99%A2)如下图所示：

![UTOOLS1580436695226.png](https://lightsmile-img.oss-cn-beijing.aliyuncs.com/UTOOLS1580436695226.png)

爬取结果如下：

```json
{"title": "山东大学信息科学与工程学院", "links": ["乌尔姆大学", "不来梅大学", "仁荷大学", "成均馆大学", "立命馆大学", "慕尼黑工业大学", "多伦多大学", "新南威尔士大学", "里昂第一大学"]}
```


## model

## embedding

## 参考

1. [smilelight/lightSpider: lightsmile个人的用于爬取网络公开语料数据的mini通用爬虫框架。](https://github.com/smilelight/lightSpider)

## 打赏

如果该项目对您有所帮助，欢迎打赏~

![UTOOLS1578660899400.jpg](https://lightsmile-img.oss-cn-beijing.aliyuncs.com/UTOOLS1578660899400.jpg)
