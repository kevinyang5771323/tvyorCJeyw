# 前言

欢迎来到本项目的Gitee页面！这是一个基于协同过滤的电影推荐系统，它使用Java语言和MySQL数据库开发而成。该项目适用于计算机专业毕业设计，提供了完整的实战项目经验，包括源码、文档报告和代码讲解。以下是项目的详细介绍。

## 内容介绍

本项目旨在为广大电影爱好者提供个性化的电影推荐服务。通过协同过滤算法，分析用户历史观影数据，挖掘出用户的偏好，从而为用户推荐可能喜欢的电影。系统采用了前后端分离的架构，后端使用Spring Boot框架提供RESTful接口，前端则运用了JS、Vue和CSS3技术实现用户交互界面。

## 技术介绍

- **语言：** Java
- **使用框架：** Spring Boot
- **前端技术：** JS、Vue、CSS3
- **开发工具：** IDEA/Eclipse
- **数据库：** MySQL 5.7/8.0
- **数据库管理工具：** phpstudy/Navicat
- **JDK版本：** jdk1.8
- **Maven：** apache-maven 3.8.1-bin
- **前端环境：** Node.Js 12\14\16

## 核心代码

以下是项目中的一部分核心代码，实现了协同过滤算法的基本功能：

```java
public List<Movie> recommendMovies(int userId, int num) {
    // 获取用户历史评分
    List<Rating> userRatings = ratingService.getUserRatings(userId);
    // 计算用户相似度
    Map<Integer, Double> similarityMap = calculateSimilarity(userId, userRatings);
    // 按相似度排序
    similarityMap = sortByValue(similarityMap);
    // 获取相似用户的评分
    Map<Integer, Double> weightedRatings = getWeightedRatings(similarityMap, userRatings);
    // 推荐电影
    return recommendBasedOnWeightedRatings(weightedRatings, num);
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/319727/36/23018/119061/689eb897Fbe544939/e9671ffc4006ffce.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/325306/1/4759/51087/689eb875F1373ee58/ec4baed60974e181.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/312497/10/26718/95095/689eb876Fe22d3fd2/d711185cdfb983a9.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/310585/38/26578/105463/689eb876Fd0282b1e/4dcc35fe6b4cf84a.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/326950/18/4829/77071/689eb877Ffd28c860/bbf948f64048fc10.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/318738/10/24936/85401/689eb878Fb3c4d1ff/0e1c65e70170f98e.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/318266/22/24961/94182/689eb878Fdc1986cf/4fe19c6c12fd0a7a.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/314704/38/26014/81212/689eb879F9e904146/8d59a29e201e4154.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/295209/10/16284/21280/689eb879F6b3e4a4f/12ee492660a99ce4.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/319172/13/25730/35603/689eb87aF185d6698/38e417343f3487de.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
