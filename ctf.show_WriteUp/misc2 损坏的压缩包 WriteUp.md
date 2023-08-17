&ensp;&ensp;&ensp;审题：一个压缩包，但试图用压缩软件（如WinRar）解压时报错，没法解压。
&ensp;&ensp;&ensp;猜测：文件本身格式出现错误。
&ensp;&ensp;&ensp;&ensp;于是用010Editor打开压缩包并观察，发现：
![图片](images/misc2_01.png#pic_center)
&ensp;&ensp;&ensp;&ensp;在阅读过Hello CTF的图片隐写相关知识点后，我们既可以从左上角的文件开头编码判断出这其实是一个png文件的文件头，也可以从右边的“译文”中推测出这其实是一个png文件。图片隐写知识点一览:https://ctf.tj.cn/ctf_misc/stego/ 。
&ensp;&ensp;&ensp;&ensp;所以把这个压缩包的后缀由.zip改为.png之后（若你的电脑看不见后缀名，则请另自行百度哈），就可以看到这个文件的原貌以及我们寻找的flag：
![图片](images/misc2_02.png#pic_center)