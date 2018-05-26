# learning NLP
# 条件分布函数
## 条件与事件
组合两个即两个以上的条件频率分布

    cfd=nltk.ConditionalFreqDist(
        (genre,word)
        for genre in brown.categories()
        for word in brown.words(categories=genre))

    genre_word=[(genre,word)
            for genre in [('news','romance')]
            for word in brown.words(categories=genre)]

# 小问题解决办法
* python 中无法显示中文解决办法：全局设置中文显示，在代码开头加上下面这一行

    # -*- coding: utf-8 -*-

#使用双连词生成随机文本
  根据每个词后面出现单词概率大小生成双连词，然后循环下去生成随机文本
  '''注意设置停止条件，防止进入死循环'''

    nltk.bigrams()



