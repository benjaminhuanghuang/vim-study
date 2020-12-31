

- Highlight
```
  :syntax on
```
- Show line number
```
  :set number
```

## Insert
a		//在当前光标位置的右边添加文本 
i		//在当前光标位置的左边添加文本 
A		//在当前行的末尾位置添加文本 
I		//在当前行的开始处添加文本(非空字符的行首) 
O		//在当前行的上面新建一行 
o		//在当前行的下面新建一行 
R		//替换(覆盖)当前光标位置及后面的若干文本 
J		//合并光标所在行及下一行为一行(依然在命令模式) 


## Navigation
- 移动光标 h j k l
```
  10 j    # 10 line up

  10 k
```
- 往前移动一个单词 w 

- 往回移动一个单词 b

- page down, ctrl + f

- page up, ctrl + n

- Jump to line 88
```  
  88 gg
``` 

## Delete
```
  x 删除当前光标下的字符
  dw 删除光标之后的单词剩余部分。
  d$ 删除光标之后的该行剩余部分。
  dd 删除当前行。

  c 功能和d相同，区别在于完成删除操作后进入INSERT MODE
  cc 也是删除当前行，然后进入INSERT MODE

  删除首行的第一个字母　：　:%s/^.//g　　貌似用键盘的 x 字母删除

```


## Search
```
  /<key>
  n            # next
  shift - n    # previous
```


## cut / pust
```
  cc          # cut current line
  u           # undo

  c2c         # cut 2 lines


  p           # paste
  u           # undo
```