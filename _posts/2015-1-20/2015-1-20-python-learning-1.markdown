---
layout: post
date: 2015-1-20
categories: itbase
---
# python learning(一)
    >>> print bin(1024)
    10000000000

    >>> map(lambda x, y, z: x+y+z, [1, 2, 3], [10, 20, 30], [100, 200, 300, 400])
    [111, 222, 333]

    >>> filter(lambda x: x!2 == 0, [1, 2, 3, 4, 5])
    [2, 4]

    >>> reduce(lambda x, y: x*y, range(1, 6))
    120

题目：输入一个英文的纯文本文件，统计其中单词出现的次数。

    def word_count(file_name):
        wc = {}
        with open(file_name, 'r') as f:
            words = f.read().split()
            for word in set(words):
                wc[word] = words.count(word)
        return sorted(wc.items(), key=lambda x:x[1], reverse=True)
