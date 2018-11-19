# -douban-
* 从豆瓣上爬取最新电影影评并进行词云显示，爬虫小白的一次简易尝试，原本为后期影评情感分析训练及未来时间节点上的情感预测做数据准备
当时的最新电影为碟中谍6，是一部还蛮精彩的电影，截止此时，豆瓣评分为8.2 
# 1.爬虫<br>
    from urllib import request<br>
    from bs4 import BeautifulSoup as bs
# 2.对标签进行解析<br>
  对子元素进行提取
# 3.数据清洗<br>
  为了方便进行数据进行清洗，将列表中的数据放在一个字符串数组中<br>
  随后正则表达式清除标点符号<br>
  清除停用词
# 4.词频统计<br>
# 5.词云进行显示<br>
    from wordcloud import WordCloud,STOPWORDS
    import matplotlib.pyplot as plt
    import pandas as pd
