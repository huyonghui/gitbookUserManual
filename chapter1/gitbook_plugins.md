# 第三节 gitbook插件


<!-- toc -->
## 配置

```json
{
    "title": "gitbookUserManual", # 标题
    "author" : "huyonghui"
    "description": "how to use gitbook.", # 描述
    "language": "zh", # 语言
    "root": ".", # 指定存放 GitBook 文件（除了 book.json）的根目录
    "plugins":[
        "3-ba", //百度统计
        "anchors" //标题带有 github 样式的锚点。
        "atoc" // 插入 TOC 目录。

        "disqus", // 添加 disqus 评论插件。
        "editlink" // 内容顶部显示 编辑本页 链接。
        "expandable-chapters" // 收起或展开章节目录中的父节点。
        "github", // 在右上角显示 github 仓库的图标链接
        "-highlight", // 默认的代码高亮插件，通常会使用 prism 来替换
        "image-captions"　// 抓取内容中图片的 alt 或 title 属性，在图片下面显示标题。
        "latex-codecogs" // 使用数学方程式
        "links", // 在左侧导航栏添加链接信息
        "mermaid"
        "prism", // 基于 Prism 的代码高亮。
        "redirect" // 页面跳转。
        "sectionx" // 分离各个段落，并提供一个展开收起的按钮。
        "sharing", // 默认的分享插件。
        "sitemap", // 生成站点地图。
        "splitter",　// 录和右侧内容之间添加一个可以拖拽的栏，用来调整两边的宽度
        "spoiler", // 隐藏答案，当鼠标划过时才显示
        "tbfed-pagefooter", // 自定义页脚，显示版权和最后修订时间。
        "todo" //待办事项        
        ],
    "pluginsConfig":{
        "3-ba": {
            "token": "a9787f0ab45d5e237bab522431d0a7ec"
        },
        "atoc": {
            "addClass": true,
            "className": "atoc"
        },
        "disqus":{
            "shortName":"gitbookUserManual"
        },
        "editlink": {
            "base": "https://github.com/huyonghui/gitbookUserManual/",
            "label": "编辑本页"
        },
        "expandable-chapters":{},
        "github":{
            "url":"https://github.com/huyonghui/gitbookUserManual"
        },
        "image-captions": {
          "caption": "Image - _CAPTION_"
        }
        "links" : {
            "sidebar" : {
            "Home" : "https://github.com/huyonghui"
            }
        }
        "sectionx": {
          "tag": "b"
        }
        "sharing": {
            "facebook": true,
            "twitter": true,
            "google": false,
            "weibo": true,
            "instapaper": false,
            "vk": false,
            "all": [
                "facebook", "google", "twitter",
                "weibo", "instapaper"
            ]
        },
        "sitemap": {
            "hostname": "https://github.com/huyonghui"
        },
        "tbfed-pagefooter": {
            "copyright":"Copyright © huyonghui 2017",
            "modify_label": "该文件修订时间：",
            "modify_format": "YYYY-MM-DD HH:mm:ss"
        }
    }
}
```

## mermaid

```mermaid
graph TD
  A-->B
  A-->C
  B-->D
  C-->D
```
## latex-codecogs

Inline math: $$\int_{-\infty}^\infty g(x) dx$$


Block math:

$$
\int_{-\infty}^\infty g(x) dx
$$

## spoiler
```
This is a spoiler: {%s%}Hello World.{%ends%}
```
