# qrHTML
这是一些常见的图片无法复制，另存为的解决方案
把下面这段代码复制到地址栏，然后按回车键。之后就可以复制当前页面了。 
javascript:alert(document.onselectstart = document.oncontextmenu= document.onmousedown = document.onkeydown= function(){return true;}); 
很多资料性的网络文章，往往在网页禁止使用“复制”、“粘贴”命令。

其解决方法如下：

方法一、最简单的破解方法： 单击IE浏览器的“工具”——“internet选项”——“安全”，将其中的“internet”的安全级别设为最高级别，“确定”后刷新网页即可。

安全级别最高的时候，一切控件和脚本均不能运行，再厉害的网页限制手段统统全部作废。 

方法二、破解网页不能复制的方法 

但对有些网页却不管用因为他们并不用脚本限制我们的(好象起点就是这样)，他们在网页中加了如下代码 
禁止左键 〈body onselectstart="return false"〉 
禁止右键 〈body oncontextmenu=self.event.returnvalue=false〉 
结合起来禁止左右键 
〈body oncontextmenu=self.event.returnvalue=false onselectstart="return false 
左右键被禁止了自然无法复制什么的了,在浏览器里查看源文件，搜索oncontextmenu.false之类的代码删除，再刷新就可以了. 
一般禁止网页复制的代码就是在<body>里加入以下代码: 
<body oncontextmenu="return false" onselectstart="return "> 

解决办法就是先把网页另存为，保存在本地之后，再对本地的那个页面用记事本编辑，把上面这段代码去掉就可以复制内容了. 
方法三、破解网页不能复制的方法：用word破解 

某些网页中的文字无论用什么方法都不能选中复制。因为被禁止复制了，如果要得到其中的某段文字，虽然可以用降低安全级别、查看源文件等方法来实施，但我们还可以用常用的Word来更为简单方便的获取. 

首先复制网页地址，然后打开Word，依次单击“文件／打开”，弹出“打开”窗口。在“文件名”中用“Ctrl+V”粘贴入已复制的网页地址，再单击“打开”按钮，这里Word就会自动连接到网站。在打开网页之前，可能会弹出“Word 没有足够的内存，此操作完成后无法撤消。是否继续？”的提示窗口，单击“是”，即弹出新的窗口，询问是否信任文件来源，再单击“是”后，Word会自动链接到对应的服务器并打开网页，这时我们就可以选中其中的文字进行复制粘贴了。另外，此法在WPS2005中也可以使用，操作起来十分方便. 

方法四、把下面这段代码复制到地址栏，然后按回车键。之后就可以复制当前页面了。javascript:alert(document.onselectstart = document.oncontextmenu= document.onmousedown = document.onkeydown= function(){return true;}); 

方法五、使用邮件功能（以 outlook 为例）： 

在浏览器快捷工具栏中中有一个邮件工具，点击后选择“发送网页”，这时候会启动outlook，并自动创建一个新邮件，邮件内容即为网页内容，这时候就可以在里面选择和复制所需要的内容了。当然也可以依次选择“文件”→“发送”→“电子邮件页面”，同样可以在outlook中打开所需要的页面并进行复制、编辑. 
方法六、使用网页编辑软件： 

浏览器有默认的网页编辑软件（一般为frontpage或者word），只要在快捷工具栏中点击相应的按钮，或者依次选择“文件”→“使用Microsoft Frontpage （或者Microsoft Word）编辑”，即可在相应软件的编辑窗口中显示网页的全部内容，这个时候就可以进行复制或修改了 

让你的问题迎刃而解

