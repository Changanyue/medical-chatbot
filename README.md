# medical-chatbot
前端界面展示的医疗聊天机器人  
基于医疗知识图谱、文本相似度和seq2seq生成模型
由于数据集和训练参数过大 并未上传

# 说明
本项目是在前端界面显示，基于医疗知识图谱+bert文本相似度+seq2seq attention的中文聊天机器人

# 运行效果
![image] https://github.com/Changanyue/medical-chatbot/blob/master/效果展示.gif

或视频：
国内bilibili：https://www.bilibili.com/video/BV1Re411W7LX/

国外YouTube：https://www.youtube.com/watch?v=Vjo8qHwGIAg&feature=youtu.be

# 配置环境
python3  
java-sdk 
neo4j

# 运行

本项目用到了百度nlpAPI，用户需要先注册申请自己的api-key。

在命令行启动neo4j服务后，再运行启动3个接口api1/2/3.py，然后打开index，进入网页。

# 代码架构
详细见项目报告.pdf

主函数：

main

主函数做成三个接口：

api1/2/3

知识图谱：

question_classifier.py

question_parser.py

answer_search.py

build_medicalgraph.py

文本相似度seq2seq模型：

sim_seq.py

seq2seq模型的一些文件：

word_token.py

training_chatbot.py

get_stopwords.py

data_utils.py

config.py

bm25_fitness_data.py
