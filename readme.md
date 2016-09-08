ulti-zh-doc
===========

[UltiSnips](https://github.com/SirVer/ultisnips)是我非常喜欢的vim插件之一，
它真的非常强大，而且非常流畅。

我希望更多人能够方便的使用UltiSnips，于是我做了这个汉化版的UltiSnips文档。翻译尚
未完成，这只是半成品，而且目前翻译的比较粗糙，我会首先完成翻译，然后做一些语义上
的优化，不至于读起来感觉很怪异。

__注意__: 这仅仅只UltiSnips的文档的翻译，到[这里](https://github.com/SirVer/ultisnips)
获取UltiSnips插件的相关信息

如果你觉得这个翻译帮助到了你，可以给我个 __star__ 。也欢迎指出我的翻译中的问题。

---

中文档的安装使用方法
--------------------

假设你正在使用[Vundle](https://github.com/gmarik/Vundle.vim)，可以直接添加下面
的配置到你的 `.vimrc` 中，如果是使用的其他插件管理器，请调整为对应的格式

    Plugin 'Linfee/ultisnips-zh-doc'

__注意:__你需要先加载 ultisnips-zh-doc 再加载 UltiSnips 才能保证打开中文文档。

---

UltiSnips简介
-------------

UltiSnips是vim代码片段终极解决方案。特有很多特性并且运行非常流畅。

![GIF Demo](https://raw.github.com/SirVer/ultisnips/master/doc/demo.gif)

这个演示中，我正在编辑一个python文件。我首先展开了`#!`片段，然后是`class`片段。
补全菜单使用的是[YouCompleteMe](https://github.com/Valloric/YouCompleteMe)，
UltiSnips同样集成了[neocomplete](https://github.com/Shougo/neocomplete.vim)。我可
以在各个插入点之间跳跃并插入文本，同时还会在代码片段的其他位置自动插入文本：当
我添加`Animal`作为一个基类，`__init__`方法会同时更新，添加调用基类的构造器的代码，
当我添加一个参数到构造器中，它会自动被赋值给实例变量。然后我插入了我的个人的代码
片段，`print`用来调试。注意我离开了插入模式，插入了另一个代码片段，然后又回来给
`__init__`方法添加了一个新的参数，而此时类的代码片段依然是激活的并且添加了另一个
实例变量。

UltiSnips的官方主页是在 <https://github.com/sirver/ultisnips>.
你可以在这里提交 pull request 和 issues。

UltiSnips于2009年6月由@SirVer创建。在2015年12月，维护工作移交给了
[@seletskiy](https://github.com/seletskiy).

你可以使用UltiSnips来干什么?
----------------------------

高级代码片段:
* [Snippets Aliases](doc/examples/snippets-aliasing/README.md)
* [Dynamic Tabstops/Tabstop Generation](doc/examples/tabstop-generation/README.md)

快速开始
--------

这里假定你正在使用 [Vundle](https://github.com/gmarik/Vundle.vim)，你可以把这些
加到你的`.vimrc` 中来安装UltiSnips，如果是其他插件管理器，请调整为对应的格式。

    " 这句放到你的插件列表中
    Plugin 'SirVer/ultisnips'

    " 代码片段和核心是分开，如果你想要默认代码片段，也加上这行
    Plugin 'honza/vim-snippets'

    " 有关触发代码片段的配置，如果你使用了 YouCompleteMe 就不要使用 tab 了
    let g:UltiSnipsExpandTrigger="<tab>"
    let g:UltiSnipsJumpForwardTrigger="<c-b>"
    let g:UltiSnipsJumpBackwardTrigger="<c-z>"

    " 如果你希望使用 :UltiSnipsEdit 的时候可以垂直切分你的窗口来编辑
    let g:UltiSnipsEditSplit="vertical"

这里有非常详尽的 UltiSnips 文档
[documentation](https://github.com/SirVer/ultisnips/blob/master/doc/UltiSnips.txt).

当然，这里还有中文版文档
[文档](https://github.com/Linfee/ultisnips-zh-doc/blob/master/doc/UltiSnips_zh.txt).


截屏
----

这里发布了一些高级用法的截屏：

- [Episode 1: What are snippets and do I need them?](http://www.sirver.net/blog/2011/12/30/first-episode-of-ultisnips-screencast/)
- [Episode 2: Creating Basic Snippets](http://www.sirver.net/blog/2012/01/08/second-episode-of-ultisnips-screencast/)
- [Episode 3: What's new in version 2.0](http://www.sirver.net/blog/2012/02/05/third-episode-of-ultisnips-screencast/)
- [Episode 4: Python Interpolation](http://www.sirver.net/blog/2012/03/31/fourth-episode-of-ultisnips-screencast/)

[Vimcasts](http://vimcasts.org) 上有三集非常优秀的讲述 UltiSnips 的视频：

- [Meet UltiSnips](http://vimcasts.org/episodes/meet-ultisnips/)
- [Using Python interpolation in UltiSnips snippets](http://vimcasts.org/episodes/ultisnips-python-interpolation/)
- [Using selected text in UltiSnips snippets](http://vimcasts.org/episodes/ultisnips-visual-placeholder/)
