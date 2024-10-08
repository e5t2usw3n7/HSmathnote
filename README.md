# Welcome to My Notes!

## 主要内容

预计是加入高中数学中**圆锥曲线的二级结论**和**导数题型**的相关知识点，同时可能会附上相关模拟题或高考题作为例题，如果后续有变动则另外附上。

## 搭建目的

- 首先，众所周知现在的教辅资料**溢价严重**，而我个人认为知识不应当用太过昂贵的代价获得，所以整理这份笔记帮助更多同学以更小的代价获得知识；
- 其次，市面上资料芜杂，至少光是本地区一片的资料都几乎**没有完整的体系归纳**，这使得很多同学到最后只知道刷了题而不知变通，这是本笔记想要解决的一点；
- 最后，因为圆锥曲线和导数板块往往出现在压轴题（尽管新高考可能发生变化），所以本笔记也是为了更好地拿下**中上难度乃至上等难度**的题。

## 联系作者

邮箱：e5t2usw3n7@outlook.com

## 关于作者

- 我是一名平凡的毕业生，很多东西不太能写得好，如果有看不懂的部分请及时发邮件与我联系，我愿尽绵薄之力回答您的问题，邮件请取名“【提问】......”；
- 若笔记存在疏漏，还望您海涵，请勘误后通过邮件联系我修改，邮件请取名“【勘误】......”；
- 若愿意分享您的优秀例题或结论补充，可以不限形式（照片、文字等）地发送在我的邮箱中，邮件请取名“【分享】......”；
- **我是个懒人，可能会拖更**。

## 网站搭建

本网站采用`mkdocs`进行搭建，这个生成器相当简洁且实用，主要使用`pymarkdown`渲染`markdown`，然后`html`渲染文件。

### 1.安装与准备

`mkdocs`是 python 的一个库，可以用`pip install mkdocs`或`pip3 install mkdocs`下载。

```shell
# 创建一个叫 note 的文件夹
$ mkdocs new note    
# 进入笔记文件夹
$ cd note
```

若您未将 python 的库加入环境变量，请在所有`mkdocs`有关命令前加上`python -m`，例如：`python -m mkdocs new note`。

此时若您能使用`tree`命令查看结构的话，您能大致看到：
```
./
├── docs/
│     └── index.md
├── mkdocs.yml
└── site/
```

### 2.配置与查看

初始化阶段准备成功后就可以进行同步渲染了，这里请先写好 mkdocs.yml 的相关内容，关于如何写这个配置文件，请移步[配置文件——mkdocs中文文档](https://hellowac.github.io/mkdocs-docs-zh/user-guide/configuration/)

```shell
# 写好以后，在本地进行同步的渲染
$ mkdocs serve
...
# “ctrl + 单击链接”即可打开渲染的网站
INFO    -  [xx:yy:zz] Serving on http://127.0.0.1:8000/
...

# 生成静态网页代码
$ mkdocs build

# 根据配置文件 mkdocs.yml 自动生成网页有关的 site 文件夹，它自己会传到 gh-pages 分支
$ mkdocs gh-deploy
```
