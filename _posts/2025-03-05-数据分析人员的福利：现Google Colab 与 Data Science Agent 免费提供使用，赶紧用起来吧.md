数据分析人员的福利：现Google Colab 与 Data Science Agent 免费提供使用，赶紧用起来吧

![image-20250305172658911](https://img.wangms.com/blog/image-20250305172658911.png)

图片中的链接如下，大家可以自行查看。本文从涉及到的服务说起，然后进行一个简单使用介绍。

https://developers.googleblog.com/en/data-science-agent-in-colab-with-gemini/?linkId=13237992

一、

数据集，google官方推荐使用的数据分析的数据来源，我认为这个网站很强大，它有好多免费的数据，我们可以利用这些数据做好多事情，尤其适合小公司或独立开发者。我甚至认为，它是本篇文章最有价值的内容。

https://www.kaggle.com/

Kaggle 是一个数据科学竞赛平台和在线社区，为数据科学家、机器学习从业者等提供了丰富的资源与服务，在人工智能和数据科学领域影响力较大。已被Google收购。

开始演示如何获取数据

1、

找到左侧datasets菜单，找个感兴趣的点击进去。

![image-20250305175031951](https://img.wangms.com/blog/image-20250305175031951.png)

2、

我准备下载2024年Spotify播放量最高的歌曲进行分析

![image-20250305175330504](https://img.wangms.com/blog/image-20250305175330504.png)

二、

Google Colab

https://colab.google/

Google Colab是一个免费的云托管 Jupyter Notebook 环境，您可以在其中直接在浏览器中编写和运行 Python 代码。它免费提供对 Google Cloud GPU 和 TPU 的访问，这对于运行 AI 模型来说是一个重大改变，并简化了项目协作。

利用Colab对刚下载的数据进行分型

1、

访问Google Colab后打开一个新的笔记本

![image-20250305175727253](https://img.wangms.com/blog/image-20250305175727253.png)

2、

使用Gemini分析文件

![image-20250305175915431](https://img.wangms.com/blog/image-20250305175915431.png)

上传文件，并发送一些分析数据的对话内容

![image-20250305180117054](https://img.wangms.com/blog/image-20250305180117054.png)

3、

Gemini收到我的消息后会给出具体的执行步骤，我们浏览下没问题选择「执行方案」

![image-20250305180431063](https://img.wangms.com/blog/image-20250305180431063.png)

4、

左侧会不断的输出代码、文字、图表，经过短暂的等待，数据分析基本完毕，我们重点看他给出的结论

![image-20250305181043898](https://img.wangms.com/blog/image-20250305181043898.png)

左侧的结论会是英文，你可以复制出来继续给Gemini让他给一个中文版本的总结。

5、

最后的一些建议想法，我们可以把数据分析的这个事分成三部分

1、提出问题

2、AI根据问题进行分析

3、得出结论

其中第二部现在已经被AI全部实现，那1、3步我们可以深入和研究下。

例如第一步，我们可以利用对数据的了解或是专业知识先和AI沟通下，让deepseek等AI大模型帮我生成一套与AI更好沟通的指令。

像这样：

你是xx专业的资深从业者，现在我有xx数据需要分析，请你帮我给出合适的与Gemini沟通的指令，你需要注意如下几点

1、

2、

3、

....

还有第三步分析的结果，你可以根据分析结果，再次利用AI帮助你完成，例如进行一些数据处理脚本的生成、缺失数据的收集...

简单介绍到这里，大家自己体验研究吧，有什么问题留言与我沟通吧