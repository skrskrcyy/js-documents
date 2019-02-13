# 概述

在本篇文章的开始，我先为大家解释一下这三个名词的概念。

px全称为pixel——像素。pc及移动设备的屏幕就是通过往像素矩阵中填充颜色，从而在宏观上体现出图像。***像素越小，图像越清晰***。

分辨率又称解析度.解像度，***其意义为该屏幕中能够显示的像素个数，往往用水平和垂直像素个数来衡量。***

ppi全称为pixels per inch，意义是***每英寸所拥有的像素个数***。由px的定义可以得出，***ppi越大，图像越清晰。***

---

# px所需要思考的问题

相同的px个数，如10px，在不同类型的显示屏幕上的物理长度相同吗？相同的px个数，在不同类型的显示屏幕中占的比例相同吗？

先回答上面的问题——***大部分情况下不相同。***

为什么呢？在这里要明确一点——***px不是物理长度单位。***其实由我概述中说的：

> 像素越小，图像越清晰

就可以看出像素大小是不确定的。

那么如何知道该显示屏下像素的大小呢——***用该屏幕的ppi值计算出来。***

公式为：***像素物理长度 = 1/ppi，单位为英寸。***

由此，我们可以知道了——***当不同类型的屏幕的单个像素物理长度不同时，相同的px个数物理长度不同。***

同时，众所周知的，分辨率有好多种，如1280×720，1920×1080等。例如1280×720，其意义就是***该屏幕水平方向由1280个像素，垂直上有720个像素。***

所以，由此可得——***当不同类型的屏幕的水平及垂直方向上的像素个数不同时，相同的px个数，在该屏幕的水平，垂直方向上所占的比例是不同的。***

---

# 进一步的思考及解决方案

通过以上的内容学习，大家应该就能理解为什么相同的px个数，在不同类型的屏幕下——尤其pc端到移动端——字体大小不同、屏幕边缘部分留白或过长失真了吧。

但是，光用px来构建网站是远远不够的。因为我们期望的是同一个网站，在不同的终端上有1.一致性，2.响应式——这两者其实是对立的，***一致性是不同终端页面内容及布局都是相同的，响应式是根据终端类型改变来改变布局以使页面更友好***——的特点，不希望有比例失真或屏幕内容过小过大的情况。

而解决这些问题，我们通常使用rem，em，自适应式建站，响应式建站。

篇幅所限，在下一章中再来讨论。

---

# 参考资料

1. 市场常见屏幕尺寸以及分辨率：[https://wenku.baidu.com/view/42bedab284254b35effd3416.html](https://wenku.baidu.com/view/42bedab284254b35effd3416.html )
2. 为什么同样大小的像素在移动端和pc端看起来不一样:[https://www.jianshu.com/p/4583755b4f69](https://www.jianshu.com/p/4583755b4f69)
