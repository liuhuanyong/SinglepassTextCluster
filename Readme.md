# 项目的背景
SinglepassTextCluster, an TextCluster tool based on Singlepass cluster algorithm that use tfidf vector and doc2vec，which can be used for individual real-time corpus cluster task。基于single-pass算法思想的自动文本聚类小组件，内置tfidf和doc2vec两种文本向量方法，可自动输出聚类数目、类簇文档集合和簇类大小，用于自有实时数据的聚类任务。

# 项目的由来


# 项目的构成 
1、data：待处理文本。  
2、model: token_vector.bin，预先训练好的字向量，可用于文本的快速向量化。  
3、result: 最终聚类结果文件，文件以json格式保存，记录聚类结果id、类簇中文本数量、类簇文本集合信息。  
4、cluster_demo.py：聚类主控脚本，在该脚本中可直接指定聚类阈值，聚类的方法和聚类输入、输出文本路径。
5、cluster_doc2vec.py：基于doc2vec的主控聚类接口。  
6、cluster_tfidf.py：基于tfidf的主控聚类接口。  
7、singlepass_cluster_tfidf.py：基于tfidf的single-pass聚类算法实现细节。   
8、singlepass_cluster_doc2vec.py：基于doc2vec的single-pass聚类算法实现细节。   

# 项目的总结
1、针对用户自有实时文本数据，利用聚类方法进行自动的文本聚类，得到聚类主题以及聚类的相关文档，可以为数据集文本的分析提供较好的帮助。基于single-pass算法思想的自动文本聚类小组件，可以直接使用。   
2、singlepass聚类算法是一个简单、快速的聚类算法，其核心在于文档向量化方法以及聚类阈值，本工具内置tfidf和doc2vec两种文本向量方法，阈值可作为超参供用户指定输入。 
3、文档向量化方法，有其他的更好的建模方法，如LDA聚类方法、bert向量化、word2vec向量化方法。  

# 关于作者
刘焕勇，liuhuanyong，现任360人工智能研究院算法专家，前中科院软件所工程师，主要研究方向为知识图谱、事件图谱在实际业务中的落地应用。
得语言者得天下，得语言资源者，分得天下，得语言逻辑者，争得天下。  
1、个人主页：https://liuhuanyong.github.io  
2、个人博客：https://blog.csdn.net/lhy2014/  
3、个人公众号：老刘说NLP  
欢迎对自然语言处理、知识图谱、事件图谱理论技术、技术实践等落地应用的朋友一同交流。
