# SYSU Beamer Unofficial

本 beamer 模版旨在为中大学子提供一个 presentation 的样式。

## 版权声明
- 本模版基于 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.en) 协议开发，您可以自由地在任何媒介以任何形式复制、使用和修改本模版，只需给出适当的署名。**注意：本模版不是官方模版。**

- 本模版的 logo 由[《中山大学视觉形象识别系统手册》](http://home3.sysu.edu.cn/sysuvi/index.html)里的素材导出，见：[http://home3.sysu.edu.cn/sysuvi/index.html](http://home3.sysu.edu.cn/sysuvi/index.html)

- 物理与天文学院的 logo 见：[https://spa.sysu.edu.cn/zh-hans/article/290](https://spa.sysu.edu.cn/zh-hans/article/290)

## 如何使用
- [Overleaf](https://www.overleaf.com/latex/templates/sysu-beamer-unofficial/zqbdzvrgkwvw)
- 直接食用 (**TeX Live 版本为 2021 及以上，否则报错**)：
    ```
    \documentclass{beamer}

    \usepackage[theme=dark,color=sysugreen,tpage=2]{sysubeamer}

    % 中文模式使用 XeLaTeX 编译器，并且使用 ctex 宏包，如：
    \usepackage[UTF8]{ctex}

    \title[Short Title]{Normal Title}
    \subtitle{Subtitle}     % optional
    \author{Your Name}
    \school{Your School}    % optional
    \date{\today}

    \begin{document}
    
    \maketitle

    \setcounter{framenumber}{0}

    \section{Introduction}

    \begin{frame}
        Your frame contents.
    \end{frame}
    \end{document}
    ```
- 3个宏包选项，第一个选项设置为默认值：
    - `theme`：主题模式，可选值为 `light` 或 `dark`
    - `color`：主题颜色，可选值为 `sysugreen`、`sysured`、`sysublack` 或 `spablue`。**注意：此选项会影响 logo 图片**。
    - `tpage`：标题页样式，可选值为 `1`、`2` 或 `3`，见: [`tpage=1`](figure/tpage1.pdf)、[`tpage=2`](figure/tpage2.pdf)、[`tpage=3`](figure/tpage3.pdf)

## 如何替换主题颜色和 logo

- 使用命令 `\def\secsym{<symbol>}` 可以自定义目录中的章节符号。
- 使用命令 `\def\themecolor{<color>}` 重新定义主题颜色为您喜欢的颜色。
- 如果您想使用其他 logo，请按照以下代码在导言区重新定义命令：
    ```
    \def\logo{<path to logo.png>}
    \def\motto{<path to motto.png>}
    \def\horizontal{<path to horizontal.png>}
    \def\vertical{<path to vertical.png>}
    \def\updown{<path to updown.png>}
    ```
**以上自定义命令意味着：您可以将此模版用作为任意高校的模版，只需将主题颜色和 logo 图案改变即可。**

- 最简单粗暴的方法是将 `logo` 文件夹中对应图片的命名替换为你的图片。

## 联系方式

- 如果对这个模板有任何问题，请随时通过以下方式联系我：
    - email: [yanghw8@mail2.sysu.edu.cn](mailto:yanghw8@mail2.sysu.edu.cn)
    - QQ 群: 929324613
    - Github: [https://github.com/yanghw8](https://github.com/yanghw8)
- 祝您使用愉快！
