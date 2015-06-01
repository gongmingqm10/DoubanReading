##豆瓣读书API文档

**1.首页科技、爱情、校园 模块**

首页科技

```
GET https://api.douban.com/v2/book/search?tag=科技&count=3
```
Response

```
{
count: 3,
start: 0,
total: 200,
books: [...]
}
```
首页爱情

```
GET https://api.douban.com/v2/book/search?tag=爱情&count=3
```

首页校园

```
GET https://api.douban.com/v2/book/search?tag=校园&count=3
```

**2.分类页面不同类别**

使用静态数据: [名著, 散文, 诗歌, 人文, IT, 漫画, 文学, 情感]

页面中显示效果如设计稿: [世界名著, 散文随笔, 诗歌, 人文社科, IT, 漫画绘本, 文学, 情感与成长]

搜索：`GET https://api.douban.com/v2/book/search?tag=名著&count=20`


**3.搜索页面**

关键字搜索，假设关键字为`文学` API如下：

```
GET https://api.douban.com/v2/book/search?q=文学&count=20
```

**4.详情页面**

显示图书详情信息 `GET  https://api.douban.com/v2/book/:id`

**5.More**

参考 [豆瓣图书API](http://developers.douban.com/wiki/?title=book_v2)