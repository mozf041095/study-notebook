# Emacs的使用
## 历史与基本概念
* 使用Lisp语言编写，是Editor MACros的缩写
* 跨平台性，适用于Unix类、Windows、iOS等
* 缓冲区：文件工作副本，可用C-x C-w/C-x C-s保存写入文件
## 快捷键
* 简记：C-Ctrl; M-Alt; C-x C-c 先Ctrl+x再Ctrl+c； C-x k 先Ctrl+x，再松手按k
* M-s：新建一个缓冲区
* C-x O：在缓冲区切换
* C-g：取消当前操作
* C-x u：回到上一步
* C-x C-3：把缓冲区分成左右两个，新缓冲区是复制当前
* C-x C-3：把缓冲区分成上下两个，新缓冲区是复制当前
* M-w：选中文字时是复制文字，没选中文字则复制当前行
* C-w：选中文字时是剪切文字，没选中文字则剪切当前行
* M-x：调出命令输入，能后接命令
* C-y：粘贴
* C-x C-s:保存文本
* C-x C-f：打开文本，不存在则新建
* C-x C-v:打开文件，代替当前缓冲区
* C-x k：关闭当前缓冲区
* C-s：前向搜索
* C-r：后向搜索
* C-x h：全选
* C-v：向下翻页
* M-v：向上翻页
* C-f：前进一个字符
* C-b：后退一个字符
* M-f：前进一个单词
* M-b：后退一个单词
* C-@：标记开始区域
* C-a：移动到行首
* C-e：移动到行尾
* M-a：移动到句首
* M-e：移动到句尾
* M-<：缓冲区头部
* M->：缓冲区尾部
* M-g M-g,num：跳转至第几行
* C-x 0：关闭当前缓冲区
* C-x C-c：退出
* 命令行模式：`emacs -nw`
## 显示行号
* M-x linum-mode
## 自动补全插件
* 名字：[company-mode](http://company-mode.github.io/)
* 安装步骤：调出命令M-x；输入list-packages，回车；出现的列表点company；点击install；点击Yes



## 引用与资料
* [程序猿助手](https://www.cnblogs.com/blfshiye/p/4566900.html)
* [Emacs精通指南](https://github.com/redguardtoo/mastering-emacs-in-one-year-guide/blob/master/guide-zh.org)
* [从零开始](https://www.jianshu.com/p/b4cf683c25f3)
