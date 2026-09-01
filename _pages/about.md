---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

大家好！我是**王菡悦**，目前是硕士一年级学生，就读于至[浙江大学计算机科学与技术学院](http://www.cs.zju.edu.cn/)。
我对人工智能充满热情，自入学以来，积极参与各类科研项目和学术竞赛，曾获得中国近现代感恩科学家奖学金（全学院仅1个名额）、ACM-ICPC银牌等多项校内外奖项。在科研方面，我参与并主导了多个项目，包括但不限于**时间序列**、**大语言模型**等领域。硕士期间研究方向为**内容安全**、**Deepfake**。

# 🎓 Education Background

- **排名：** GPA排名：**1/819 (0.12%)**、综测排名：**1/819 (0.12%)**  
- **成绩均分：** GPA：4.3/5.0、加权平均分：93/100  
- **语言能力：** 已通过 CET4 和 CET6，《计算机专业英语》成绩为94分，曾独立撰写并投稿全英文学术论文  
- **核心课程：** 高等数学 (100)、线性代数 (94)、概率论与数理统计 (95)、离散数学 (98)、程序设计基础 (95)、Python (97)、Java (96)、Web程序设计 (92)、数据结构与算法分析 (96)、人工智能 (99)、软件工程 (95)、ICS (91)、操作系统 (94)、数据库 (93)、计算机网络 (93)、网络与信息安全 (98)  
- **编程能力：** 熟练掌握 C++ 和 Python，熟悉算法与数据结构，代码能力强，曾获 ACM-ICPC 银牌；熟练掌握 PyTorch、Numpy、Pandas，熟悉各类深度学习模型及其编程实现；长期担任数学建模编程手，曾获“高教社杯”全国大学生数学建模竞赛省级特等奖  
- **开发工具：** VS Code, PyCharm, Jupyter Notebook, LaTeX (Overleaf), Git  
- **在校荣誉：** 曾获第六届中国近现代感恩科学家奖学金（全学院仅1个名额）、三好学生标兵、国家奖学金

# 🔥 News

# 📈 Research Experience-Time Series

## **💡💡💡 TempoStackNet - A Novel Cryptocurrency Price Prediction Framework**  

- **时间：** 2023.3 - 2024.3  
- **领域：** **时间序列预测**，**AI for Finance**  
- **角色：** 第一作者  
- **研究背景：**  
  1. 相较于传统投资市场，加密货币市场由于其动态性和高波动性，使得相关的价格预测方法效率较低，现有方法无法应对市场的投机性和复杂性。
  2. 当前亟需一种高效的价格预测方法，以更准确地预测加密货币的价格趋势。
- **我们的方法：**  
  1. **引入TempoStackNet框架：** 我们设计了一种新颖的加密货币价格预测框架TempoStackNet，结合了叠加集成学习和跨时间窗口策略，利用时序注意力机制，整合192/96/48个时间窗口间隔的历史数据，有效提高了多步价格预测的准确性。
  2. **多步价格预测策略：** 通过高精度预测未来32天内的加密货币价格趋势，显著提升了预测模型的泛化性和鲁棒性。
- **项目成果：**  
  * 在Global Technology and Cryptocurrency Volatility、S&P 500指数等多个数据集上的实验结果显示，TempoStackNet在准确性、泛化性和鲁棒性方面优于现有的SOTA方法。

## **💡 Kaggle: Optiver - Trading at the Close** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/optiver-trading-at-the-close) | [[Leaderboard]](https://www.kaggle.com/competitions/optiver-trading-at-the-close/leaderboard)</sub>  

- **时间：** 2023.11 - 2024.1  
- **领域：** **时间序列预测**，**AI for Trading**  
- **角色：** 团队(主力队员)  
- **研究背景：**  
  1. 股票交易以高波动性和快速的价格变化为特征，特别是在纳斯达克交易所，每个交易日都以收盘交叉拍卖结束。该过程确定了证券的官方收盘价格，是市场参与者评估市场表现的关键指标。
  2. 在交易的最后十分钟，做市商会将传统订单簿数据与拍卖簿数据相结合，提供最佳的价格参考。在这次比赛中，挑战在于开发一个模型，利用订单簿和收盘拍卖数据来预测数百支纳斯达克股票的收盘价走势。
- **我们的方法：**  
  1. **特征工程：** 进行特征转换，处理时序数据（如时间特征提取、滚动窗口统计等），并进行特征选择。
  2. **回归算法测试：** 尝试多种回归算法（如CatBoost、XGB、LGBM、神经网络等），最终确定LGBM与神经网络为最佳模型。
  3. **超参数优化：** 使用Grid Search和Randomized Search方法分别进行超参数优化，综合考虑后选取合适的超参数。
- **项目成果：**  
  * 取得了5.4724的最终分数，获得铜牌(Top 6%)。

# 🧩 Research Experience-Large Language Models

## **💡 Kaggle: LMSYS-Chatbot Arena Human Preference Predictions** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/lmsys-chatbot-arena) | [[Leaderboard]](https://www.kaggle.com/competitions/lmsys-chatbot-arena/leaderboard)</sub>  

- **时间：** 2024.5 - 2024.8  
- **领域：** **大语言模型**，**LLM问答**  
- **角色：** 团队(主力成员)  
- **研究背景：**  
  1. 本次竞赛的挑战是预测用户在两个人工智能对话系统（LLM）之间的对决中更偏爱哪个回答。参赛者将获得一组来自Chatbot Arena的对话数据，这些对话是由不同的LLM生成的。
  2. 通过开发一个获胜的机器学习模型，目标是改进聊天机器人与人类的互动方式，使其更符合人类的偏好。
- **我们的方法：**  
  1. **模型选择与测试：** 最初测试了Deberta base、Deberta v2、Xlarge、Deberta v3 large等“小语言”模型，效果不佳。参考公开方案和讨论区观点后，转向“大语言”模型测试。
  2. **大语言模型尝试：** 尝试了Gemma2 9b，Gemma2 27b，Llama3 8b模型。Gemma2 27b在本地测试表现最佳，但因超出比赛环境GPU显存限制，最终选择Gemma2 9b和Llama3 8b模型。
  3. **微调与集成：** 使用QLoRA对两个模型进行微调，尝试两种方案：[对Gemma2 9b设置较高的Rank（32,64）微调作为单模型]和[对Gemma2 9b和Llama3 8b均设置较低的Rank（16）进行微调，最后集成]，最终选择了集成方案。
- **项目成果：**  
  * 取得了0.98739的最终分数，获得银牌(Top 2%)。

# 🏆 Competition Awards

- **Kaggle: Chatbot Arena Human Preference Predictions：银牌** *国家级* 2024  
- **Kaggle: LLM-Detect AI Generated Text：铜牌** *国家级* 2024 
- **Kaggle: Optiver - Trading at the Close：铜牌** *国家级* 2024 
- **中国国际“互联网+”大学生创新创业大赛(全国总决赛)：银奖** *国家级* 2023  
- **全国大学生软件创新大赛(全国总决赛)：三等奖** *国家级* 2024 
- **全国大学生数学建模竞赛：特等奖** *省部级* 2023 
- **中国国际“互联网+”大学生创新创业大赛(省级赛)：金奖** *省部级* 2023 
- **全国大学生软件创新大赛(西北赛区)：一等奖** *省部级* 2024 
- **国际大学生程序设计竞赛(ACM-ICPC)：银牌** *省部级* 2023 
- **中国大学生服务外包创新创业大赛(西部区域赛)：三等奖** *省部级* 2024 

# 🥇 Scholarships and Honors

- *2021-2022* **中国近现代感恩科学家奖学金** 
- *2023-2024* **三好学生标兵** 
- *2024-2025* **国家奖学金** 
