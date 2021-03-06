---
title: Music Classification
localeTitle: 音乐分类
---
## 音乐分类

音乐分类是另一个可以应用深度学习策略的领域，以获得比传统机器学习方法更高的分类精度。最初用于图像识别和计算机视觉任务的深度神经网络可以通过使用频谱图用于音乐分类。频谱图只不过是一段时间内音乐中频率频谱的直观表示。换句话说，作为合成频率的音乐信号可以被分成其频谱，并且可以在视觉上为每个频率表示以dB为单位的响度。该图像可用于训练对这些谱图进行分类的神经网络。一个很好的用例是类型识别。

### 以下是各种光谱图的示例：

![Spectrogram1](http://deepsound.io/images/new_blues_00.png)

上面的谱图是来自布鲁斯类型的歌曲。频率沿y轴，时间沿x轴。较亮的颜色表示该频率的声音是响亮的，而较暗的颜色表示它们在那些特定的时间点是柔和的。包含如此多数据的这种图像可用于训练神经网络。我们通常使用mel-scaled谱图来进行类型识别，这是由听众判断的音高范围，即我们如何感知这些频率以区分各种类型的组成部分。

**傅里叶变换**

需要知道的一个重要细节是，这种频谱图是在称为傅立叶变换的数学概念的帮助下创建的。傅里叶变换将时间函数分解为构成它的频率。

#### 更多信息

如果您使用的是python，则有许多用于信号处理的库。 [Librosa](https://librosa.github.io/librosa/)是一个着名的，另一个是[scipy](https://scipy.org/) ，也可以用于其他科学目的。利用这些库可以创建mel谱图。

##### 有关上述主题的更多信息，请查看以下链接：

*   [寻找类型](https://hackernoon.com/finding-the-genre-of-a-song-with-deep-learning-da8f59a61194)
*   [Deepsound](http://deepsound.io/music_genre_recognition.html)