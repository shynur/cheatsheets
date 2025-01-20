<https://www.bilibili.com/video/BV1Bv4y1J7QT?p=6>

# 参考

[Quick Reference (GNU make)](https://www.gnu.org/software/make/manual/html_node/Quick-Reference.html)

# 概念
## Rule

Makefile 主要由 *rule*s 组成, 一条 *rule* 形如:

``` makefile
target: dependencies ...
	commands
	...
```

## Comment

从 `#` 往后都是单行注释.
在少部分情况下 `#` 会被解释为 string, 因此不要到处乱用.
`\#` 被解释为 `#` 字面量.

# 命令行 options

- `-o FILE`: 强迫 make 将 FILE 当成是 未被更改的旧文件.

# Conventions and Template

``` makefile
SHELL = /bin/bash
.SUFFIXES: .exe  # 我习惯给可执行文件加此后缀.
```




<!-- Local Variables:                         -->
<!-- eval: (electric-quote-local-mode -1)     -->
<!-- whitespace-style: (face tabs)            -->
<!-- eval: (whitespace-mode)                  -->
<!-- markdown-gfm-recognized-languages: t     -->
<!-- markdown-fontify-code-blocks-natively: t -->
<!-- End:                                     -->
