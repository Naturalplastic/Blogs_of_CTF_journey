&ensp;&ensp;&ensp;审题：一张png图片，那应该是misc杂项之png隐写类型题。
&ensp;&ensp;&ensp;&ensp;图片隐写知识点一览:https://ctf.tj.cn/ctf_misc/stego/ 。
&ensp;&ensp;&ensp;&ensp;考虑到这是萌新签到第一题，应该比较直白。
&ensp;&ensp;&ensp;&ensp;用010Editor查看图片后，发现并无知识点一览中的那几种png隐写特殊情况，故考虑其他知识点。
&ensp;&ensp;&ensp;&ensp;在图片所在文件夹下打开cmd，执行指令strings <文件名>，即strings misc1.png，可以查看图片里隐含的所有字符串。在众多无规律字符串中，我们注意到了如下一个显眼的家伙：
![图片](images/misc1_01.png#pic_center)
&ensp;&ensp;&ensp;&ensp;这就是我们要找的flag，将一整行复制（dos窗口的复制快捷键是右crtl+insert，粘贴是右shift+insert）并粘贴至提交窗口提交即可。