# pgf - Create PostScript and PDF graphics in TeX

http://ctan.org/pkg/pgf


PGF是用于生成图的宏包。它独立于平台和格式，与最重要的TeX终端驱动共同工作，包括pdfTeX和dvips。与之并生的用户友好的语法层TikZ。

它的用法同于pstricks和标准图环境。PGF在plain (pdf-)TeX，(pdf-)LaTeX，和ConTeXt中均有效。和pstrics不同的是，它可以生成PostScript或PDF输出。


本项目文档来自于：http://mirrors.ctan.org/install/graphics/pgf/base/pgf.tds.zip

在zip压缩包中`/doc/generic/pgf/`含有所有手册原文件，置于`doc-en`中，相应的中文翻译在`doc-zh`中。


## 文档结构

- 每种编译版本文档，在`version-for-XXX`之中。
- 文档正文在`text-en`中，也正是我们翻译的目标内容。

## 操作

### 翻译

大家若认领其中的内容，填加相应章节题目，勾选其中内容即可。

- [x] Introduction
- [ ] Part I Tutorials and Guidelines
+ [ ] Tutorial: A Picture for Karl’s Students
     * [ ] Problem Statement
     * [ ] Setting up the Environment 
     * [ ] Straight Path Construction
     * [ ] Curved Path Construction
     * [ ] Circle Path Construction
     * [ ] Rectangle Path Construction
- [ ] Part II Installation and Configuration
- [ ] Part III  ik Z ist kein Zeichenprogramm
- [x] Part IV Graph Drawing
- [x] Part V Libraries
- [ ] Part VI Data Visualization
- [ ] Part VII Utilities
- [ ] Part VIII Mathematical and Object-Oriented Engines
- [ ] Part IX The Basic Layer
- [ ] Part X The System Layer
- [ ] Part XI References and Index

### 编译

Till Tantau为我们提供了非常便捷的编译方式——`Makefile`(在每个版本文件夹中，如`/doc-zh/version-for-xetex/en/`)：

- 在终端键入命令`make`即实现编译。
- 键入`make clean`即清除临时文件。
- 完整编译整个手册非常耗时，可建立一个工作分支，在当前分支上注释掉`pgfmanual-en-main-body.tex`中的大部分非关注内容。待测试通过后再编译全部文档，并合并到主分支上。

        git branch current
        git checkout current
        # 翻译、编辑正文
        git add .
        git commit -m "some comments"
        git checkout master
        git merge current

## 联系人

未尽事宜，请来信垂询：[yangdawei.hit@qq.com](yangdawei.hit@qq.com)

翻译交流QQ群：390651602
