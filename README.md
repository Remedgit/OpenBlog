# WRITE BY REMEDGIT!
## 开放博客-HTML
这个项目就是我目前正在使用的博客，因为githubpage不开放仓库需要开plus，所以如果有人想用，就不用改我的代码了(也属于是被迫开源了吧)。当然我不确定有人会用

我们毕业了，我在家闲的没事，把我自己和gpt一起写的（我先让gpt生成了一个博客模版，然后对照着mdui.org的文档一步步改成了现在的样子，你可以看到，一些html里面有一些空的Style css样式，这就是gpt留下的史山，删了就炸，明明mdui改完之后不需要了......）博客简单（指花费两个小时）修改了一下，让那些想搭建GithubPages 博客的人fork一下
## 介绍一下这个Blog的结构
### 单个文件
- index.html
这个用来判断手机电脑访问然后自动跳转的
- computer.html
电脑访问网页

添加文章:添加到 /article后面
```html
<div class="mdui-col">
      <div class="mdui-grid-tile">
        <img src="#"/>
        <div class="mdui-grid-tile-actions">
          <div class="mdui-grid-tile-text">
            <div class="mdui-grid-tile-title">#</div>
            <div class="mdui-grid-tile-subtitle"><i class="mdui-icon material-icons">account_circle</i>by Remedgit OpenBlog using mdreader-beta</div>
          </div>
          <div class="mdui-grid-tile-buttons">
            <button class="mdui-btn mdui-btn-icon" onclick="window.location.href='#'"><i class="mdui-icon material-icons">arrow_forward</i></button>
          </div>
        </div>
      </div>
    </div>
```
- mobile.html
手机访问网页 ⚠️史山警告！

添加文章:
```html
<div class="mdui-card">
          <div class="mdui-card-header">
            <img class="mdui-card-header-avatar" src="#">
            <div class="mdui-card-header-title">#</div>
            <div class="mdui-card-header-subtitle">#</div>
          </div>
          <div class="mdui-card-media">
            <img src="#">
          </div>
          <div class="mdui-card-primary">
            <div class="mdui-card-primary-title">Title</div>
          </div>
          <div class="mdui-card-content">subtitle</div>
          <div class="mdui-card-actions">
            <button class="mdui-btn mdui-ripple" onclick="window.location.href='#'">SeeMore</button>
          </div>
</div>
<br>
```
- about.html
关于你自己的界面，自己修改

- notice.html
网站公告

公告放置在/notice:
```html
<article class="mdui-ripple mdui-hoverable">
    <h2>Title</h2>
    <p>subtitle</p>
    <br>
    <p>subsubtitle</p>
    <p>subsubsubtitle / Date</p>
</article>
```

### 文件夹
- fileserver
这里存放让观众下载的文件
- src
这里存放博客里出现的图片资源
- article
# 重磅级
## MDREADER.html
这个东西花费了我两三天的时间，我让gpt帮帮我结果生成了一个啥也用不了的东西，最后还是我和gpt一起改的，让markdown在html里渲染，目前处于Beta版本

文章放置于article文件夹内，访问https://你的网站.github.io/article/mdreader.html?read=###.md 这里###.md就是你的md文件名字
- files
也是放一些文件用的
## 使用方法
Fork这个仓库，然后自己改代码，githubpage大家应该都会用