# miniblink49
=======================================================
本次开源的代码未经许可，禁止用于商业用途

关于miniblink的介绍见这篇文章：https://zhuanlan.zhihu.com/p/22611497?group_id=764036386641707008

一、关于编译
========================================================
1、目前编译尽量使用VS2015以上的编译器,否则可能出现未知错误

2、Release版本默认采用VC6运行时库,此特性可以通过USING_VC6RT宏控制

3、miniblink默认同时导出CEF和WKE两种接口,导出接口可以通过ENABLE_CEF和ENABLE_WKE两个宏控制.#这里至少选择一种导出接口
二、关于说明
========================================================
1、miniblink主要是用来做PC端的浏览器嵌入组件，由于导出的是wke和cef的接口，所以你可以替换到你的项目中去体验和学习。基本相当于一个wke的升级版本，或者cef的精简版。

2、代码其实比较挫，很多地方为了能尽快跑起来，加了N多断点，以及很难看的代码····所以大家尽情批判，我会逐步改掉。

3、代码里我觉得最复杂的是cc目录，那个是我自己写的，一个简单的软件渲染合成层。现在的blink，已经不是当年的webkit了，没有这个目录，连绘制都绘制不了。。

4、代码里被我有意和无意的加了些坑，所以想用在项目上，估计有点点麻烦。

5、目前我在搞M53了，所以这次开源的是M49的。但也算比较新的内核了。

6、下一步的发展方向是electron的接口，以及把M49的功能补充完整。目前缺少挺多功能的，比如前进后退还没做；UI线程和blink主线程还是同一根线程；还没写透明窗口；
三、关于讨论
========================================================
大家有问题可以加群178168957、或者邮箱weolar@qq.com，或者csdn：blog.csdn.net/weolar ,或者github里留言讨论。
当然我不会所有问题都回答的，毕竟还要去工地搬砖养家糊口。

最后特别感谢zero，他帮我提交了很多代码。
