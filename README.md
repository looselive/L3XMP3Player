# L3X MP3 Player

![Screenshot](https://github.com/lexrus/L3XMP3Player/raw/master/l3xmp3player.png)

这是 2003 年我初学 Flash 时做的 MP3 播放器。用到的数字液晶字体是我自己做的，界面是我用 Fireworks 设计的。虽然源码已经跟着我的老电脑一起消失了，但是编译后的 swf 在网上广为流转，[直到现在还有一些网站在用](https://www.google.com/#hl=en&q=l3x+mp3+player)。

## 怎样使用

* 下载相关文件(swf,xml)，下然完成后上传至你的网站

* 在你的html文件中插入如下代码


    <object classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase=" http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab #version=6,0,29,0 " width="165" height="120">
    <param name="movie" value="plugin/mp3player.swf">
    <param name="quality" value="low">
    <param name="wmode" value="transparent">
    <param name="menu" value="false">
    <embed src="plugin/mp3player.swf" quality="low" pluginspage=" http://www.macromedia.com/go/getflashplayer " type="application/x-shockwave-flash" width="166" height="120"></embed>
    </object>


替换你上传的swf的地址
注: 为了呈现出像素效果，quality 参数必须设置成 low

* 编辑 mp3list.xml，并上传对应的 mp3 文件


    <?xml version="1.0" encoding="UTF-8"?>
    <mp3>
        <I n="IRIS" f="mp3/iris.mp3" a="GOO GOO DOLLS"/>
        <I n="十年" f="mp3/tenyears.mp3" a="陈奕迅"/>
        <I n="Don't You Forget" f="mp3/dontyouforget.mp3" a="ERA"/>
    </mp3>


每个 i 标签即指定一份 mp3 文件, n 属性指定歌名, f 属性指定对应的mp3文件地址, a 属性为可选, 指定专辑名
注: mp3list.xml 使用 UTF-8 编码


## LICENSE

Copyright (C) 2012 LexTang.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.