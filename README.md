## 神说，要有光。于是...

梦回2019，那时我刚接触输入法方案，像开启了一扇新大门，原来五笔方案还能这么玩？！

于是我打算自己尝试制作，而这一做，就是两年..

没错，陆陆续续，曲曲折折才算把第一版做好，于是便有了下面的故事：

# 大道至简 - 阴阳平衡 - 一阴一阳之谓道矣。。

## 		-191五笔（aka 19音形）

​						音の力 53% 形の力 47%

传统五笔几大痛点是什么？

- 难学，难记，不常用字根学了又忘
- 拆分恶心，不符合习惯（实际上我明白制作人的难点）
- 花这么大功夫学习了五笔，什么？！还有重码！不能忍不能忍，哈哈

于是，为什么生活不能是美好而简单的呢？

为什么需要重复造轮子，重复记忆一些东西，而仅仅为了打字？！

哈，

所以，都说路径依赖不好，但我们可以依赖已有的认知，比如五笔祖师爷86，比如我们小学义务教育的拼音。。

于是就有了191五笔。

在部分影响较小的字根上沿袭86的布局，而对于比较难拆的，则采用拼音编码，具体如下：

字根大体分为三类，一类是传统86字根，按照86布局；

二是拼音编码，如我 -> wo，非 -> fei, 方 -> fan，为什么方最后少了个g？因为我的单字最高只有3码。。

第三类是键名汉字，遵照86重复编码方式。

准确讲对于单字的编码可以用以下这个规则：

if 是拼音字：

​	其声母首字母 + 韵母首字母 + 韵母次字母，最多3码

elif 是非拼音，非键名字:

​	第一笔字根 + 第二笔字根 + 第三笔字根（不足三笔字根的采用这个的声母首字母填充）

else:

​	其他有键名字，极少数几个特殊编码的字，见excel。

方案整体采用3码空间内搞定单字与3字词，并且3字词总是在3码前几位的，并且单字分布在一码空间 + 二码空间 + 三码空间，选3重，推荐使用逗号句号选重。

4码空间只有2字词和4字词及以上词。

用2简词，但因为其实191有较大缺陷，就是4码重码率有点高，所以暂时先维护到这，二简词还未加入词库。大家可以把它当玩具或参考学习娱乐下。

具体的参照excel或issue区评论。

参照阅读：https://www.bilibili.com/video/BV1DK4y1H75c

QQ群：972385384

todo

- [ ] 192五笔纯打词极致方案
- [ ] 19五笔系列方案辅助练习软件（初版会制作一个REPL命令行界面辅助学习19五笔）

2021.01.23创立
