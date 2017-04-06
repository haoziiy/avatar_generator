# avatar_generator
哈希头像图片生成器 Python代码

Identicon 在很多大型IT网站上可以见到,比如 Github, Sourceforge, Stackoveflow 等等,
 刚刚注册的账号的个人信息的默认图标​都​是​一​些​看​上​去​像​七​巧​板​拼​凑​的​图​案​,​对​称​又​变​化​多​端​。

以 Github 为例， Github 给无头像用户生成 5x5 像素的 Identicons 头像。
这一生成过程使用了用户ID的哈希值，然后根据哈希值每一位的奇偶值来决定对应位置上的像素的开关。
这样生成 的图像，配上由哈希值决定的颜色，保证可生成大量独一无二的图像。



![](http://identicon.net/img/identicon.png)
哈希头像事例：http://identicon.net

根据哈希算法，本项目代码可以通过运行test_batch文件会在相同的目录保存多个png格式的图片。
````
img= identicon.render_identicon(code, 16)
````
这里的code是一个数值, 或者字符串数值, 如果code比较大, 比如code=10000000, 生成的图片就是彩色的.
code比较小, 比如code=1~100之间的, 生成的图片就是黑白色的.




