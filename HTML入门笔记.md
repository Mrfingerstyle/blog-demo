# HTML入门笔记
### HTML 是谁发明的

    Tim Berners-Lee 李爵士

### HTML 起手应该写什么

    <!-- 文档类型 -->
    <!DOCTYPE html>
    <!-- html根标签 zh-CN -->
    <html lang="zh-CN">
****
    <head>
        <!-- 文件字符编码 -->
        <meta charset="UTF-8">
        <!-- 禁用缩放 兼容手机 -->
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <!-- 告诉IE使用最新内核 -->
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Demo</title>
    </head>

    <body>
    </body>

    </html>

### 常用的表章节的标签有哪些，分别是什么意思

- h1~h6 标题 从 h1 - h6 字体大小一次减小
- section 章节
- article 文章
- main 主要内容
- aside 旁支内容

### 全局属性有哪些

- 所有标签都有的属性
- class 类
- contenteditable 可编辑的
- hidden 隐藏
- id id 属性 其实并不唯一代表元素
- style 设置 css 的属性
- tabindex tab 索引 设置浏览网页时使用 tab 健切换元素的顺序
- title 标题 鼠标悬停时显示的内容

### 常用的内容标签有哪些，分别是什么意思

- a 超链接
- strong 重要 加粗 本身很重要
- em 强调 默认样式是斜体 语气很重要 强调成分
- code 显示代码 不换行 和 pre 配合使用可换行
- pre 保留 空格 tab 回车的样式
- ol li 有序列表
- ul li 无序列表
- dl dt dd 自定义列表
- hr 分割线
- br 换行
- quote 内联
- blockquote 块级引用
