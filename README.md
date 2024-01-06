# medium10mostread

<<<<<<< HEAD
medium阅读量最高的10篇翻译

## Medium software-engineering 文章阅读量前10翻译

即：https://medium.com/tag/software-engineering

## 思路

1. https://medium.com/tag/software-engineering 如果分析点赞即怕手图标前10的文章，要么抓取这个标签下所有的用户，通过用户api直接获取。 过程如下：

   * 获取此tag下所有用户 考虑爬虫

   * 通过用户名拿userId https://medium.com/@hnasr?format=json

   * 通过userId拿 totalClapCount https://medium.com/_/api/users/e4cbe924ccb/profile/stream?limit=25

2. 爬取 https://medium.com/tag/software-engineering 所有文章，统计后获取拍手计数入数据库，找出前10的文章

3. 直接翻译网站提供的 https://medium.com/tag/software-engineering 历年所有阅读量前10的文章，调用免费的谷歌翻译

### 下面实现第3种方案，主要实现翻译，生成PDF对应中英文文件。

页面提供的选择有 https://medium.com/tag/software-engineering/archive 10 most read 和 All years选项，因为这10 篇文章有涉及付费阅读，这里选取一篇的一个段落翻译用着例子。

### 功能简介

1. 填入通过规则获取的文章url，拉取整个页面生成pdf文件
2. 注册百度翻译api https://api.fanyi.baidu.com/register
3. 中英文逐段对照，可根据段落符号生成一段原文再生成一段翻译产生在新的pdf文件中

### 参考说明

https://github.com/aszx87410/medium-user-crawler

https://github.com/Humoonruc/translate-pdf-node

=======
>>>>>>> d1ba6d8 (init)
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
