# HTML常用标签
### a 标签的用法

    属性
        href
        target
        download 理论上是下载目标网页 不是查看那个网页 有的浏览器不支持
        rel=noopener js阶段
    作用
        跳转到外部页面
        跳转到内部锚点
        跳转到邮箱或电话

    两种开启后台服务器的方法
        在当前页面建立一个服务器 不要缓存 http-server . -c-1
        使用parcel也可以 parcel a.html

    手机访问开启的服务器
        手机和电脑在同一个局域网下
        手机访问 服务器的网址

    href取值
        网址
            https://google.com
            http://google.com
            //google.com
            <a href="https://google.com">google</a>
            <a href="http://google.com">google</a>
            <a href="//google.com">google</a>

        路径
            /a/b/c 及 a/b/c
            index.html ./index.html
            <a href="/a/b/c.html">c.html</a>
            <a href="a/b/c.html">c.html</a>
            在哪里开启的服务 哪里就是根目录
            此处的 / 不是文件的根目录 而是http服务的根目录
            如果没有 / 只是a/b/c.html 表示在相对路径 在当前路径下找a b c.html
            结果是一样
        协议
            javascript
            mailto
            tel
        id
            href=#xxx

        在当前页面找index.html
            <a href="index.html">index</a>
        或者加./ 效果一样
            <a href="./index.html">index</a>

        伪协议
        早期使用 现在基本不用
            <a href="javascript:alert(1);">javascript伪协议</a>
        空的伪协议 什么都不做
            <a href="javascript:;">空的伪协议</a>

        刷新效果
            <a href="">查看</a>

        回到顶部效果 不刷新
            <a href="#">回到顶部</a>

        内部锚点
        跳转到制定的标签
            <a href="#xxx">内部锚点</a>

        发邮件
            <a href="mailto:XXXXXXXX@qq.com">发邮件</a>

        打电话
        在手机上可用
            <a href="tel:12345">打电话</a>

### img 标签的用法

    src 属性
        网络地址 或 相对路径 绝对路径

    img 标签会发起get请求 获取图片

    alt 加载失败时显示

    width height 宽 高
        只写宽度 高度会自适应
        只写高度 宽度会自适应
        宽 高 全部设置 图片会变形
        前端的底线 永远不要让图片变形

    事件 onload onerror
        xxx.onload = function () {
        console.log("图片加载成功");
        }
        // 图片加载失败的时候显示另一张图片
        xxx.onerror = function () {
        console.log("图片加载失败");
        xxx.src = "/404.jpg";
        }

    如何做响应式
        max-width: 100%;

### table 标签的用法

    thead
    tbody
    tfoot
    三者顺序可以改变
    tr th
    tr table row
    没有写tbody 浏览器自动加上tbody

    相关的样式
        table-layout

### 其他感想

    HTML标签很多 需要循序渐进学习
