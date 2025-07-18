# Proxy-Share-Website
一个代理节点的分享网站设计，使用css和html基本语法，有透明毛玻璃效果，能够自定义文本和背景以及设计
## HTML文件在Releases中！！！
以下是更改方法和托管到C***DF***E的方法（小白友好型）
1. 修改内容：

标题：修改 <h1> 标签内的文本
公告内容：修改 <p>📢 最新公告：...</p> 的文本
链接地址：修改所有 copyText() 函数中的链接
配置项标题：修改 <h3> 标签内的文本
2. 更换背景：

找到 :root 变量中的 --bg-image
将URL替换为您自己的图片地址（推荐使用https链接）
3. 修改字体：

在 <head> 部分修改Google Fonts链接
在 body 的 font-family 中替换字体名称
4. 调整颜色：

修改 :root 中的 --glass-bg（背景透明度）
修改 --glass-border（边框颜色）
修改按钮背景色 #4f46e5
Cloudflare Pages部署教程

Cloudflare Pages部署界面参考

步骤：

访问 Cloudflare Pages
点击左侧菜单的 Pages
点击 创建项目
连接您的Git账户（GitHub/GitLab）
选择您的代码仓库（可以新建空仓库）
构建设置：
Framework preset: 选择 HTML Only
Build command: 留空
Build output: 留空
点击 部署站点
自定义域名：

进入项目页面
点击 自定义域
输入您的域名（需在Cloudflare管理）
等待DNS生效（约1-10分钟）
技术说明
响应式设计：使用媒体查询和弹性布局，适配手机/平板/电脑 [7]
毛玻璃效果：通过 backdrop-filter 实现现代设计 [6]
复制功能：使用Clipboard API并包含错误处理 [1]
字体适配：使用Google Fonts实现跨平台字体 [8]
常见问题
背景不显示：检查图片链接是否为HTTPS且有效
复制功能异常：确认使用HTTPS访问（本地文件需开启本地服务器）
自适应问题：所有容器宽度已设置百分比适配
Cloudflare部署失败：确保仓库为空或包含正确文件结构
