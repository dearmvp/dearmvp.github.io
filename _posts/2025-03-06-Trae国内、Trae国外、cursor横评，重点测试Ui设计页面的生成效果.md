最近浏览网络信息时，发现大家有在用claude-3.7做UI设计的，效果是真的好，堪比专业设计，甚至有网友直接可以生成Figma识别的原型图。更有网友直接充当设计人员接单赚钱了。

正好前几天Trae发布国内版本，我利用这个想法对比下Trae国内、Trae国外、Cursor的效果。

先说结论

因为都使用的是chat模式，所以似乎和IDE关系不大，顶多是每个IDE对集成的模型调教匹配度的区别，从下面的UI效果图上看也如网友所说的一样claude-3.7效果是真的好，deepseek R1 和claude-3.5如果再进行几轮对话，应该也会出现理想的效果。

下面是详细介绍

Trae-国内-doubao-1.5

特意说明下，doubao1.5生成的页面不是一个页面展示三个UI效果图。下面的图片是我手动截图拼接在一起后的效果，看每个效果图都有滚动条就明白了

所以，先不说UI效果看着是否舒服，最起码对指令的理解还是有问题

![image-20250306144004392](https://img.wangms.com/blog/image-20250306144004392.png)

Trae-国内-deepseek-r1

特殊说明：下方图也是手动将三个UI效果图拼接在一起的，所以结论和上面的一样，理解指令有问题。但UI效果图比上边的要美观些

![image-20250306144532320](https://img.wangms.com/blog/image-20250306144532320.png)

Trae-国内-deepseek-chat-v3

你没看错，deepseek-chat-v3就给生成一个页面，不仅理解有问题，UI效果图也不太美观，说明它真不适合代码类生成。

![image-20250306145711155](https://img.wangms.com/blog/image-20250306145711155.png)

Trae-国外-claude-3.7

这没什么好评价的，上面结论已经说了，确实效果很不错，我指令要求的是参考apple设计风格，看来他很了解apple的风格，走极简风格路线了，我看网上有让他参考一些欧美风，视觉效果很炫的风格，他给生成的也确实很炫。

![image-20250306150106939](https://img.wangms.com/blog/image-20250306150106939.png)

Trae-国外-claude-3.5

大致是把效果实现出来了，但和3.7生成的效果相比还有很多细节要处理。如果进一步沟通应该可以达到效果。

![image-20250306150359196](https://img.wangms.com/blog/image-20250306150359196.png)

Trae-国外-gpt-4o

效果比claude3.5还差一些，但可以理解指令，效果美观上差很多。

![image-20250306150719236](https://img.wangms.com/blog/image-20250306150719236.png)

Trae-国外-deepseek-R1

同样是手动拼接在一起的UI效果图，设计效果也不是很好，和Trae国内版生成的效果接近。

![image-20250306151004691](https://img.wangms.com/blog/image-20250306151004691.png)

Cursor-claude-3.7

效果和Trae-国外-claude-3.7 基本一致，连录音时间都一样(02:34)，哈哈

![image-20250306145840955](https://img.wangms.com/blog/image-20250306145840955.png)

以上是相同的指令，不同的IDE，不同的模型，都使用chat模式，完全在没进行二次交流的情况下生成的效果。

测试到这里，我发现生成的效果和IDE没多大关系，就不继续测试了。按目前情况，大家如果要做UI设计直接选claude 3.7就行，退而求次就选deepseek R1和claude-3.5 

要求免费的话就用Trae国内版，然后使用deepseek R1模型，国内版本的claude-3.7可能会排队，估计等一段时间大家都可以顺畅的免费的使用了。



在我测试完这些内容后，我重启了下国外版的Trae然后发现国外版的IDE把国内版集成的两个模型也加入进来了。所以如果在使用国外版的Trea就没必要再下载柜内版Trae了。

![image-20250306161952808](https://img.wangms.com/blog/image-20250306161952808.png)

PS：把Trae用国内、国外区分不知道是否恰当，准确的说我表述的国外版是从https://www.trae.ai/这里下载的，字节最先发布的AI IDE

国内版是从https://www.trae.com.cn/这里下载的，字节前几天发布AI IDE