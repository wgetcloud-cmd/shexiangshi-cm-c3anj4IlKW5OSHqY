
# 一.gsap动画库


## 1\.1 基本使用和原理


首先直接npm安装然后导入


比如让一个物体，x轴时间为5s


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedGIF.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedGIF.gif)


旋转同理


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128214756914.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128214756914.png)


动画的速度曲线，可以在官网的文档找到


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215002275.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215002275.png)


## 1\.2 控制动画属性与方法


当然这里面也有一些方法，动画完成，动画开始等


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215200803.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215200803.png)


**一些属性**


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215321286.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215321286.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedGIF.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedGIF.gif)


也可实现停止动画随时，给到一个变量


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215435858.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215435858.png)


双击暂停以及恢复


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215547134.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215547134.png)


# 二.灯光与阴影详解


添加环境光


这种光一般是用来增亮，他没有阴影效果


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215713865.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215713865.png)


[![](undefined)](undefined)


平行光：类似于太阳


默认在这个位置朝着原点打光


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215940076.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefinedimage-20241128215940076.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201054.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201054.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201346.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201346.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201967.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282201967.png)


也可以改变平行光的照射点


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282202029.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282202029.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282203102.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282203102.png)


**创建阴影四部曲**


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282204326.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282204326.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205172.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205172.png)


谁产生阴影


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205001.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205001.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205717.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205717.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205632.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282205632.png)


**注意：物体可以投射阴影，也可以接受阴影，不只是要在平面上接受**


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282206848.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282206848.png)


## 2\.1 直线光与阴影详细设置


移动球体z轴前后，出了一定范围会被剪切掉


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282258827.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282258827.png)


**平行光是有范围的**


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282259328.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282259328.png)


打印这个灯光，可以看到其范围


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282301434.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282301434.png)


far是后面，near是前面


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282301977.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282301977.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282302722.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282302722.png)


现在就比刚才更远一点，到了10的边缘才被截取


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282302724.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282302724.png)


此时这个阴影是有锯齿感的


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304455.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304455.png)


默认是512


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304779.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304779.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304606.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202411282304606.png)


## 2\.2 聚光灯


target就是聚光灯打向什么地方


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022222481.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022222481.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022222345.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022222345.png)


设置好角度之后


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022224250.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022224250.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022224489.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022224489.png)


如果想设置边缘的光慢慢衰减


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022226636.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022226636.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022225650.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022225650.png)


衰减的快慢设置


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022236602.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022236602.gif)


## 2\.3点光源


聚光灯是往一个地方发散，点光源是四面八方


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022239726.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022239726.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022239630.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022239630.png):[slower加速器](https://chundaotian.com)


点光源也可以设置距离和衰减情况


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022241677.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022241677.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022241190.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022241190.png)


# 三.透明度纹理和阴影


加入给一个物体贴上一个透明度纹理，黑色就是全透明，白色就是不透明


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022247250.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022247250.png)


此时透明度有了，但是阴影还是正常的


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022248246.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022248246.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022249684.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022249684.png)


**加上alphatest即可，此时表示大于0\.5就是透明，小于0\.5就是不透明**


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022250188.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022250188.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022250350.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022250350.png)


**此时新的问题贴上贴图后会有条纹的现象**


这是由于灯光和阴影形成的一个问题


解决方法


设置灯光阴影的bias


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022252309.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022252309.png)


偏移量，让阴影便宜一点点


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022252188.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022252188.gif)


# 四.大场景动态级联阴影设置


添加一个相机辅助器把灯光加入进来


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022255841.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022255841.png)


可以看到物体在相机范围内有阴影超过就没有阴影


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022256687.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022256687.gif)


那如果实在一个很大的场景，比如把相机的阴影场景改的很大


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022257377.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022257377.png)


会发现阴影出现了锯齿状


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022258958.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022258958.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022257290.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022257290.png)


那么此时的解决思路就是，分模块分远近来展示阴影


也就是级联阴影


类似于这样，近处的细节就比较细，远处稍微模糊点，因为距离远了也看不太清了


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022301598.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022301598.png)


导入


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022302732.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022302732.png)


需要的参数，这些都是可以直接复制threejs上面这一个图的官方例子


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022303332.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022303332.png)


然后创建级联阴影实例


maxfar表示阴影最大到多远，cascades多少个等级，mode是模式，parent当前级联阴影的父级，mapsize级联阴影的大小，lightdirection灯光的位置


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022304266.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022304266.png)


然后把所有需要设置阴影的材质都设置为级联阴影


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022306076.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022306076.png)


然后需要一直更新渲染


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022310433.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022310433.png)


此时灯管也不再需要投射阴影了交给级联来投射


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022313990.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022313990.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022313980.gif)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022313980.gif)


如果想设置灯光方向


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022314056.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022314056.png)


加上软阴影实现一个更柔滑的效果


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315969.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315969.png)


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315808.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315808.png)


前面对于灯光阴影的设置也可以不要了


[![](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315169.png)](https://heymar.oss-cn-chengdu.aliyuncs.com/undefined202412022315169.png)


  * [一.gsap动画库](#%E4%B8%80gsap%E5%8A%A8%E7%94%BB%E5%BA%93)
* [1\.1 基本使用和原理](#tid-SpfXSh)
* [1\.2 控制动画属性与方法](#tid-jWRZDe)
* [二.灯光与阴影详解](#%E4%BA%8C%E7%81%AF%E5%85%89%E4%B8%8E%E9%98%B4%E5%BD%B1%E8%AF%A6%E8%A7%A3)
* [2\.1 直线光与阴影详细设置](#tid-xzBPXE)
* [2\.2 聚光灯](#tid-him4i2)
* [2\.3点光源](#tid-YKXdTf)
* [三.透明度纹理和阴影](#%E4%B8%89%E9%80%8F%E6%98%8E%E5%BA%A6%E7%BA%B9%E7%90%86%E5%92%8C%E9%98%B4%E5%BD%B1)
* [四.大场景动态级联阴影设置](#%E5%9B%9B%E5%A4%A7%E5%9C%BA%E6%99%AF%E5%8A%A8%E6%80%81%E7%BA%A7%E8%81%94%E9%98%B4%E5%BD%B1%E8%AE%BE%E7%BD%AE)

   \_\_EOF\_\_

   ![](https://github.com/heymar)Heymar  - **本文链接：** [https://github.com/heymar/p/18598353](https://github.com)
 - **关于博主：** 评论和私信会在第一时间回复。或者[直接私信](https://github.com)我。
 - **版权声明：** 本博客所有文章除特别声明外，均采用 [BY\-NC\-SA](https://github.com "BY-NC-SA") 许可协议。转载请注明出处！
 - **声援博主：** 如果您觉得文章对您有帮助，可以点击文章右下角**【[推荐](javascript:void(0);)】**一下。
     
