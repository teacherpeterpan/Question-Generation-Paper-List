# Question-Generation-Paper-List
A summary of must-read papers for Neural Question Generation (NQG)

- Contributed by **[Liangming Pan](http://www.liangmingpan.com)** and **[Yuxi Xie](https://yuxixie.github.io/)**.

## [Content](#content)

<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#models">2. Models</a></td></tr>
<tr>
    <td>&emsp;<a href="#basic-seq2seq-models">2.1 Basic Seq2Seq Models</a></td>
    <td>&ensp;<a href="#encoding-answers">2.2 Encoding Answers</a></td>
</tr>
<tr>
    <td>&emsp;<a href="#linguistic-features">2.3 Linguistic Features</a></td>
    <td>&ensp;<a href="#question-specific-rewards">2.4 Question-specific Rewards</a></td>
</tr>
<tr>
    <td>&emsp;<a href="#content-selection">2.5 Content Selection</a></td>
    <td>&ensp;<a href="#question-type-modeling">2.6 Question Type Modeling</a></td>
</tr>
<tr>
    <td>&emsp;<a href="#encode-wider-contexts">2.7 Encode wider contexts</a></td>
    <td>&ensp;<a href="#other-directions">2.8 Other Directions</a></td>
</tr>
<tr><td colspan="2"><a href="#applications">2. Applications</a></td></tr> 
<tr>
    <td>&emsp;<a href="#difficulty-controllable-QG">2.1 Difficulty Controllable QG</a></td>
    <td>&ensp;<a href="#conversational-QG">2.2 Conversational QG</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#asking-special-questions">2.3 Asking special questions</a></td>
    <td>&ensp;<a href="#answer-unaware-QG">2.4 Answer-unaware QG</a></td>
</tr>
<tr>
    <td>&emsp;<a href="#unanswerable-QG">2.5 Unanswerable QG</a></td>
    <td>&ensp;<a href="#combining-QA-and-QG">2.6 Combining QA and QG</a></td>
</tr>
<tr>
    <td>&emsp;<a href="#QG-from-knowledge-graphs">2.7 QG from knowledge graphs</a></td>
    <td>&ensp;<a href="#visual-question-generation">2.8 Visual Question Generation</a></td>
</tr> 
<tr>
    <td>&emsp;<a href="#distractor-generation">2.9 Distractor Generation</a></td>
    <td>&ensp;<a href="#cross-lingual-QG">2.10 Cross-lingual QG</a></td>
</tr>
<tr><td colspan="2"><a href="#evaluation">3. Evaluation</a></td></tr>
<tr><td colspan="2"><a href="#resources">4. Resources</a></td></tr>
</table>

## [Survey papers](#content)
1. **Recent Advances in Neural Question Generation.** arxiv, 2018. [paper](https://arxiv.org/pdf/1905.08949.pdf)
    
    *Liangming Pan, Wenqiang Lei, Tat-Seng Chua, Min-Yen Kan.* 

## [Models](#content)   

### [Basic Seq2Seq Models](#basic-models)

Basic Seq2Seq models with attention to generate questions. 

1. **Learning to ask: Neural question generation for reading comprehension.** ACL, 2017. [paper](https://www.aclweb.org/anthology/P17-1123.pdf)

    *Xinya Du, Junru Shao, Claire Cardie.*

2. **Neural question generation from text: A preliminary study.** NLPCC, 2017. [paper](https://www.researchgate.net/profile/Franco_Scarselli/publication/4202380_A_new_model_for_earning_in_raph_domains/links/0c9605188cd580504f000000.pdf)

    *Qingyu Zhou, Nan Yang, Furu Wei, Chuanqi Tan, Hangbo Bao, Ming Zhou.*

3. **Machine comprehension by text-to-text neural question generation.** Rep4NLP@ACL, 2017. [paper](https://arxiv.org/pdf/1705.02012.pdf)
   
   *Xingdi Yuan, Tong Wang, Çaglar Gülçehre, Alessandro Sordoni, Philip Bachman, Saizheng Zhang, Sandeep Subramanian, Adam Trischler*

### [Encoding Answers](#answer-encoding)

Applying various techniques to encode the answer information thus allowing for better quality answer-focused questions. 

1. **Answer-focused and Position-aware Neural Question Generation.** EMNLP, 2018. [paper](https://www.aclweb.org/anthology/D18-1427)
   
   *Xingwu Sun, Jing Liu, Yajuan Lyu, Wei He, Yanjun Ma, Shi Wang*

2. **Improving Neural Question Generation Using Answer Separation.** AAAI, 2019. [paper](https://arxiv.org/pdf/1809.02393.pdf) [code](https://github.com/yanghoonkim/NQG_ASs2s)

    *Yanghoon Kim, Hwanhee Lee, Joongbo Shin, Kyomin Jung.*

3. **Improving Question Generation with Sentence-level Semantic Matching and Answer Position Inferring.** AAAI, 2020. [paper](https://arxiv.org/pdf/1912.00879.pdf)
   
   *Xiyao Ma, Qile Zhu, Yanlin Zhou, Xiaolin Li, Dapeng Wu*

### [Linguistic Features](#linguistic-features)

Improve QG by incorporating various linguistic features into the QG process. 

1. **Neural Generation of Diverse Questions using Answer Focus, Contextual and Linguistic Features.** INLG, 2018. [paper](https://arxiv.org/pdf/1809.02637.pdf)

    *Vrindavan Harrison, Marilyn Walker*

2. **Automatic Question Generation using Relative Pronouns and Adverbs.** ACL, 2018. [paper](https://www.aclweb.org/anthology/P18-3022)
   
   *Payal Khullar, Konigari Rachna, Mukul Hase, Manish Shrivastava* 

3. **Learning to Generate Questions by Learning What not to Generate.** WWW, 2019. [paper](https://arxiv.org/pdf/1902.10418.pdf) [code](https://github.com/BangLiu/QG)

    *Bang Liu, Mingjun Zhao, Di Niu, Kunfeng Lai, Yancheng He, Haojie Wei, Yu Xu.*

4. **Improving Neural Question Generation using World Knowledge.** arXiv, 2019. [paper](https://arxiv.org/pdf/1909.03716.pdf)
   
   *Deepak Gupta, Kaheer Suleman, Mahmoud Adada, Andrew McNamara, Justin Harris*

### [Question-specific Rewards](#RL-rewards)

Improving the training via combining supervised and reinforcement learning to maximize question-specific rewards

1. **Teaching Machines to Ask Questions.** IJCAI, 2018. [paper](https://www.ijcai.org/proceedings/2018/0632.pdf)
   
   *Kaichun Yao, Libo Zhang, Tiejian Luo, Lili Tao, Yanjun Wu*

2. **Natural Question Generation with Reinforcement Learning Based Graph-to-Sequence Model** NeurIPS Workshop, 2019. [paper](https://arxiv.org/pdf/1910.08832.pdf)
   
   *Yu Chen, Lingfei Wu, Mohammed J. Zaki*

3. **Putting the Horse Before the Cart:A Generator-Evaluator Framework for Question Generation from Text** CoNLL, 2019. [paper](https://arxiv.org/pdf/1808.04961.pdf)
   
   *Vishwajeet Kumar, Ganesh Ramakrishnan, Yuan-Fang Li*

4. **Addressing Semantic Drift in Question Generation for Semi-Supervised Question Answering** EMNLP, 2019. [paper](https://arxiv.org/pdf/1909.06356.pdf) [code](https://github.com/ZhangShiyue/QGforQA)
   
   *Shiyue Zhang, Mohit Bansal*

5. **Reinforcement Learning Based Graph-to-Sequence Model for Natural Question Generation** ICLR, 2020. [paper](https://arxiv.org/pdf/1908.04942.pdf)
   
   *Yu Chen, Lingfei Wu, Mohammed J. Zaki*

### [Content Selection](#content-selection)

Improve QG by considering how to select question-worthy contents (content selection) before asking a question. 

1. **Identifying Where to Focus in Reading Comprehension for Neural Question Generation.** EMNLP, 2017. [paper](https://www.aclweb.org/anthology/D17-1219.pdf)
   
   *Xinya Du, Claire Cardie*


2. **A Comparative Study on Question-Worthy Sentence Selection Strategies for Educational Question Generation.** AIED, 2019. [paper](https://link.springer.com/chapter/10.1007/978-3-030-23204-7_6)
   
   *Guanliang Chen, Jie Yang, Dragan Gasevic*


3. **Learning to Generate Questions by Learning What not to Generate.** WWW, 2019. [paper](https://arxiv.org/pdf/1902.10418.pdf) [code](https://github.com/BangLiu/QG)

    *Bang Liu, Mingjun Zhao, Di Niu, Kunfeng Lai, Yancheng He, Haojie Wei, Yu Xu.*

4. **Improving Question Generation With to the Point Context.** EMNLP, 2019. [paper](https://arxiv.org/pdf/1910.06036.pdf)

    *Jingjing Li, Yifan Gao, Lidong Bing, Irwin King, Michael R. Lyu.*

5. **Weak Supervision Enhanced Generative Network for Question Generation.** IJCAI, 2019. [paper](https://arxiv.org/pdf/1907.00607v1)
   
   *Yutong Wang, Jiyuan Zheng, Qijiong Liu, Zhou Zhao, Jun Xiao, Yueting Zhuang*

6. **A Multi-Agent Communication Framework for Question-Worthy Phrase Extraction and Question Generation.** AAAI, 2019. [paper](https://www.aaai.org/ojs/index.php/AAAI/article/view/4700/4578)
   
   *Siyuan Wang, Zhongyu Wei, Zhihao Fan, Yang Liu, Xuanjing Huang*

7. **Mixture Content Selection for Diverse Sequence Generation.** EMNLP, 2019. [paper](https://arxiv.org/pdf/1909.01953.pdf) [code](https://github.com/clovaai/FocusSeq2Seq)
   
   *Jaemin Cho, Minjoon Seo, Hannaneh Hajishirzi*

8. **Asking Questions the Human Way: Scalable Question-Answer Generation from Text Corpus.** WWW, 2020. [paper](https://arxiv.org/pdf/2002.00748.pdf)
   
   *Bang Liu, Haojie Wei, Di Niu, Haolan Chen, Yancheng He*

### [Question Type Modeling](#question-type-modeling)

Improve QG by explicitly modeling question types or interrogative words. 

1. **Question Generation for Question Answering.** EMNLP,2017. [paper](https://www.aclweb.org/anthology/D17-1090)
   
   *Nan Duan, Duyu Tang, Peng Chen, Ming Zhou*

2. **Answer-focused and Position-aware Neural Question Generation.** EMNLP, 2018. [paper](https://www.aclweb.org/anthology/D18-1427)
   
   *Xingwu Sun, Jing Liu, Yajuan Lyu, Wei He, Yanjun Ma, Shi Wang*

3. **Let Me Know What to Ask: Interrogative-Word-Aware Question Generation** EMNLP Workshop, 2019. [paper](https://arxiv.org/pdf/1910.13794.pdf)
   
   *Junmo Kang, Haritz Puerto San Roman, Sung-Hyon Myaeng*

4. **Question-type Driven Question Generation** EMNLP, 2019. [paper](https://arxiv.org/pdf/1909.00140.pdf)
   
   *Wenjie Zhou, Minghua Zhang, Yunfang Wu*

### [Encode Wider Contexts](#encode-wider-contexts)

Improve QG by incorporating wider contexts in the input passage. 

1. **Harvesting paragraph-level question-answer pairs from wikipedia.** ACL, 2018. [paper](https://arxiv.org/pdf/1805.05942.pdf) [code&dataset](https://github.com/xinyadu/HarvestingQA)
    
    *Xinya Du, Claire Cardie*

2. **Leveraging Context Information for Natural Question Generation** ACL, 2018. [paper](https://www.aclweb.org/anthology/N18-2090) [code](https://github.com/freesunshine0316/MPQG)
   
   *Linfeng Song, Zhiguo Wang, Wael Hamza, Yue Zhang, Daniel Gildea*

3. **Paragraph-level Neural Question Generation with Maxout Pointer and Gated Self-attention Networks.** EMNLP, 2018. [paper](https://www.aclweb.org/anthology/D18-1424.pdf)
   
   *Yao Zhao, Xiaochuan Ni, Yuanyuan Ding, Qifa Ke*

4. **Capturing Greater Context for Question Generation** AAAI, 2020. [paper](https://arxiv.org/pdf/1910.10274.pdf)
   
   *Luu Anh Tuan, Darsh J Shah, Regina Barzilay*

### [Other Directions](#other-model)

1. **Generating Question-Answer Hierarchies.** ACL, 2019. [paper](https://arxiv.org/pdf/1906.02622.pdf) [code](http://squash.cs.umass.edu/)
   
   *Kalpesh Krishna and Mohit Iyyer.*

2. **Unified Language Model Pre-training for Natural Language Understanding and Generation.** NeurIPS, 2019. [paper](https://arxiv.org/pdf/1905.03197.pdf) [code](https://github.com/microsoft/unilm)
   
   *Li Dong, Nan Yang, Wenhui Wang, Furu Wei, Xiaodong Liu, Yu Wang, Jianfeng Gao, Ming Zhou, Hsiao-Wuen Hon*

3. **Can You Unpack That? Learning to Rewrite Questions-in-Context.** EMNLP, 2019. [paper](https://www.aclweb.org/anthology/D19-1605.pdf)
   
   *Ahmed Elgohary, Denis Peskov, Jordan L. Boyd-Graber*

4. **Sequential Copying Networks.** AAAI, 2018. [paper](https://arxiv.org/pdf/1807.02301.pdf)
   
   *Qingyu Zhou, Nan Yang, Furu Wei, Ming Zhou*

5. **Let's Ask Again: Refine Network for Automatic Question Generation.** EMNLP, 2019. [paper](https://www.aclweb.org/anthology/D19-1326.pdf)
   
   *Preksha Nema, Akash Kumar Mohankumar, Mitesh M. Khapra, Balaji Vasan Srinivasan, Balaraman Ravindran*

## [Applications](#applications)

### [Difficulty Controllable QG](#difficulty-controllable-QG)

Endowing the model with the ability to control the difficulty of the generated questions. 

1. **Easy-to-Hard: Leveraging Simple Questions for Complex Question Generation.** arxiv, 2019. [paper](https://arxiv.org/pdf/1912.02367.pdf)

    *Jie Zhao, Xiang Deng, Huan Sun.*

2. **Difficulty Controllable Generation of Reading Comprehension Questions.** IJCAI, 2019. [paper](https://www.ijcai.org/proceedings/2019/0690.pdf)
   
   *Yifan Gao, Lidong Bing, Wang Chen, Michael R. Lyu, Irwin King* 

3. **Difficulty-controllable Multi-hop Question Generation From Knowledge Graphs.** ISWC, 2019. [paper](https://arxiv.org/pdf/1807.03586.pdf)  [code&dataset](https://github.com/liyuanfang/mhqg)
   
   *Vishwajeet Kumar, Yuncheng Hua, Ganesh Ramakrishnan, Guilin Qi, Lianli Gao, Yuan-Fang Li*

### [Conversational QG](#conversational-QG)

Learning to generate a series of coherent questions grounded in a question answering style conversation. 

1. **Learning to Ask Questions in Open-domain Conversational Systems with Typed Decoders.** ACL, 2018. [paper](https://arxiv.org/pdf/1805.04843.pdf) [code](https://github.com/victorywys/Learning2Ask_TypedDecoder) [dataset]( http://coai.cs.tsinghua.edu.cn/hml/dataset/)
   
   *Yansen Wang, Chenyi Liu, Minlie Huang, Liqiang Nie*

2. **Answerer in Questioner's Mind: Information Theoretic Approach to Goal-Oriented Visual Dialog.** NIPS, 2018. [paper](https://arxiv.org/pdf/1802.03881.pdf)

   *Sang-Woo Lee, Yu-Jung Heo, Byoung-Tak Zhang*

3. **Interconnected Question Generation with Coreference Alignment and Conversation Flow Modeling.** ACL, 2019. [paper](https://arxiv.org/pdf/1906.06893.pdf) [code](https://github.com/Evan-Gao/conversational-QG)
   
   *Yifan Gao, Piji Li, Irwin King, Michael R. Lyu*

4. **Reinforced Dynamic Reasoning for Conversational Question Generation.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1203) [code](https://github.com/ZJULearning/ReDR) [dataset](https://stanfordnlp.github.io/coqa/)
   
   *Boyuan Pan, Hao Li, Ziyu Yao, Deng Cai, Huan Sun*

5. **Towards Answer-unaware Conversational Question Generation.** ACL Workshop, 2019. [paper](https://www.aclweb.org/anthology/D19-5809.pdf)
   
   *Mao Nakanishi, Tetsunori Kobayashi, Yoshihiko Hayashi*

6. **What Should I Ask? Using Conversationally Informative Rewards for Goal-oriented Visual Dialog.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1646.pdf)
   
   *Pushkar Shukla, Carlos Elmadjian, Richika Sharan, Vivek Kulkarni, Matthew Turk, William Yang Wang*

7. **Visual Dialogue State Tracking for Question Generation.** AAAI, 2020. [paper](https://arxiv.org/pdf/1911.07928.pdf)
   
   *Wei Pang, Xiaojie Wang*

### [Asking special questions](#asking-special-questions)

This direction focuses on exploring how to ask special types of questions, such as mathematical questions, open-ended questions, non-factoid questions, and clarification questions. 

1. **Are You Asking the Right Questions? Teaching Machines to Ask Clarification Questions.** ACL Workshop, 2017. [paper](https://www.aclweb.org/anthology/P17-3006.pdf)
   
   *Sudha Rao*

2. **Automatic Opinion Question Generation.** ICNLG, 2018. [paper](https://www.aclweb.org/anthology/W18-6518.pdf)
   
   *Yllias Chali, Tina Baghaee* 

3. **A Multi-language Platform for Generating Algebraic Mathematical Word Problems.** arxiv, 2019. [paper](https://arxiv.org/pdf/1912.01110.pdf)
   
   *Vijini Liyanage, Surangika Ranathunga*

4. **Interpretation of Natural Language Rules in Conversational Machine Reading.** EMNLP, 2018. [paper](https://arxiv.org/pdf/1809.01494.pdf) [dataset](https://sharc-data.github.io/)
   
   *Marzieh Saeidi, Max Bartolo, Patrick Lewis, Sameer Singh, Tim Rocktäschel, Mike Sheldon, Guillaume Bouchard, Sebastian Riedel*

5. **Asking the Crowd: Question Analysis, Evaluation and Generation for Open Discussion on Online Forums.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1497.pdf)
   
   *Zi Chai, Xinyu Xing, Xiaojun Wan, Bo Huang*

6. **Conclusion-Supplement Answer Generation for Non-Factoid Questions.** AAAI, 2020. [paper](https://arxiv.org/pdf/1912.00864.pdf)
   
   *Makoto Nakatsuji, Sohei Okui*

7. **Answer-based Adversarial Training for Generating Clarification Questions.** NAACL, 2019. [paper](https://arxiv.org/pdf/1904.02281.pdf) [code](https://github.com/raosudha89/clarification_question_generation_pytorch)
   
   *Rao S, Daumé III H.*

8. **Distant Supervised Why-Question Generation with Passage Self-Matching Attention.** IJCNN, 2019. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8851781)
   
   *Jiaxin Hu, Zhixu Li, Renshou Wu, Hongling Wang, An Liu, Jiajie Xu, Pengpeng Zhao, Lei Zhao*

### [Answer-unaware QG](#answer-unaware-QG)

In answer-unaware QG, the model does not require the target answer as an input to serve as the focus of asking. Therefore, the model should automatically identify question-worthy parts within the passage to ask. 

1. **Learning to ask: Neural question generation for reading comprehension.** ACL, 2017. [paper](https://www.aclweb.org/anthology/P17-1123.pdf)

    *Xinya Du, Junru Shao, Claire Cardie.*

2. **Neural Models for Key Phrase Extraction and Question Generation.** ACL Workshop, 2018. [paper](https://www.aclweb.org/anthology/W18-2609.pdf)
   
   *Sandeep Subramanian, Tong Wang, Xingdi Yuan, Saizheng Zhang, Adam Trischler, Yoshua Bengio*

3. **Self-Attention Architectures for Answer-Agnostic Neural Question Generation.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1604.pdf)
   
   *Thomas Scialom, Benjamin Piwowarski, Jacopo Staiano.*

### [Unanswerable QG](#unanswerable-QG)

Learning to generate questions that cannot be answered by the input passage. 

1. **Learning to Ask Unanswerable Questions for Machine Reading Comprehension.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1415.pdf)
   
   *Haichao Zhu, Li Dong, Furu Wei, Wenhui Wang, Bing Qin, Ting Liu*

### [Combining QA and QG](#Combining-QA-and-QG)

This direction investigate how to combine the task of QA and QG by multi-task learning or joint training. 

1. **Question Generation for Question Answering.** EMNLP,2017. [paper](https://www.aclweb.org/anthology/D17-1090)
   
   *Nan Duan, Duyu Tang, Peng Chen, Ming Zhou*

2. **Learning to Collaborate for Question Answering and Asking.** NAACL, 2018. [paper](https://www.aclweb.org/anthology/N18-1141)
   
   *Duyu Tang, Nan Duan, Zhao Yan, Zhirui Zhang, Yibo Sun, Shujie Liu, Yuanhua Lv, Ming Zhou*

3. **Generating Highly Relevant Questions.** EMNLP, 2019. [paper](https://arxiv.org/abs/1910.03401)
   
   *Jiazuo Qiu, Deyi Xiong*

4. **Learning to Answer by Learning to Ask: Getting the Best of GPT-2 and BERT Worlds.** arxiv, 2019. [paper](https://arxiv.org/pdf/1911.02365.pdf)
   
   *Tassilo Klein, Moin Nabi*

5. **Triple-Joint Modeling for Question Generation Using Cross-Task Autoencoder.** NLPCC, 2019. [paper](https://link.springer.com/chapter/10.1007/978-3-030-32236-6_26)
   
   *Hongling Wang, Renshou Wu, Zhixu Li, Zhongqing Wang, Zhigang Chen, Guodong Zhou*

6. **Addressing Semantic Drift in Question Generation for Semi-Supervised Question Answering** EMNLP, 2019. [paper](https://arxiv.org/pdf/1909.06356.pdf) [code](https://github.com/ZhangShiyue/QGforQA)
   
   *Shiyue Zhang, Mohit Bansal*

7. **Synthetic QA Corpora Generation with Roundtrip Consistency** ACL, 2019. [paper](https://arxiv.org/pdf/1906.05416.pdf)
   
   *Chris Alberti, Daniel Andor, Emily Pitler, Jacob Devlin, Michael Collins*


### [QG from knowledge graphs](#QG-from-knowledge-graphs)

This direction is about generating questions from a knowledge graph. 

1. **Generating Factoid Questions With Recurrent Neural Networks: The 30M Factoid Question-Answer Corpus.** ACL, 2016. [paper](https://arxiv.org/pdf/1603.06807.pdf) [dataset](https://www.agarciaduran.org)
   
   *Iulian Vlad Serban, Alberto García-Durán, Çaglar Gülçehre, Sungjin Ahn, Sarath Chandar, Aaron C. Courville, Yoshua Bengio*

2. **Generating Natural Language Question-Answer Pairs from a Knowledge Graph Using a RNN Based Question Generation Model.** ACL, 2017. [paper](https://www.aclweb.org/anthology/E17-1036/)
   
   *Mitesh M. Khapra, Dinesh Raghu, Sachindra Joshi, Sathish Reddy*

3. **Knowledge Questions from Knowledge Graphs.** ICTIR, 2017. [paper](https://arxiv.org/pdf/1610.09935.pdf)
   
   *Dominic Seyler, Mohamed Yahya, Klaus Berberich.*

4. **Zero-Shot Question Generation from Knowledge Graphs for Unseen Predicates and Entity Types.** NAACL, 2018. [paper](https://arxiv.org/pdf/1802.06842.pdf) [code](https://github.com/NAACL2018Anonymous/submission)
   
   *Hady Elsahar, Christophe Gravier, Frederique Laforest.*

5. **A Neural Question Generation System Based on Knowledge Base** NLPCC, 2018. [paper](https://link.springer.com/chapter/10.1007/978-3-319-99495-6_12)
   
   *Hao Wang, Xiaodong Zhang, Houfeng Wang*

6. **Formal Query Generation for Question Answering over Knowledge Bases.** ESWC, 2018. [paper](https://link.springer.com/chapter/10.1007/978-3-319-93417-4_46)
   
   *Hamid Zafar, Giulio Napolitano, Jens Lehmann*

7. **Generating Questions for Knowledge Bases via Incorporating Diversified Contexts and Answer-Aware Loss.** EMNLP, 2019. [paper](https://www.aclweb.org/anthology/D19-1247.pdf)
   
   *Cao Liu, Kang Liu, Shizhu He, Zaiqing Nie, Jun Zhao*

8. **Difficulty-controllable Multi-hop Question Generation From Knowledge Graphs.** ISWC, 2019. [paper](https://arxiv.org/pdf/1807.03586.pdf)  [code&dataset](https://github.com/liyuanfang/mhqg)
   
   *Vishwajeet Kumar, Yuncheng Hua, Ganesh Ramakrishnan, Guilin Qi, Lianli Gao, Yuan-Fang Li*

9.  **How Question Generation Can Help Question Answering over Knowledge Base.** NLPCC, 2019. [paper](http://tcci.ccf.org.cn/conference/2019/papers/183.pdf)
    
    *Sen Hu, Lei Zou, Zhanxing Zhu*


### [Visual Question Generation](#visual-question-generation)

Asking questions based on visual inputs (usually an image). 

1. **Generating Natural Questions About an Image** ACL, 2016. [paper](https://arxiv.org/pdf/1603.06059.pdf)
   
   *Nasrin Mostafazadeh, Ishan Misra, Jacob Devlin, Margaret Mitchell, Xiaodong He, Lucy Vanderwende*

2. **Creativity: Generating Diverse Questions Using Variational Autoencoders** CVPR,2017. [paper](https://arxiv.org/pdf/1704.03493.pdf)
   
   *Unnat Jain, Ziyu Zhang, Alexander G. Schwing*

3. **Automatic Generation of Grounded Visual Questions** IJCAI, 2017. [paper](https://www.ijcai.org/proceedings/2017/0592.pdf)
   
   *Shijie Zhang, Lizhen Qu, Shaodi You, Zhenglu Yang, Jiawan Zhang*

4. **A Reinforcement Learning Framework for Natural Question Generation using Bi-discriminators** COLING, 2018. [paper](https://www.aclweb.org/anthology/C18-1150.pdf)
   
   *Zhihao Fan, Zhongyu Wei, Siyuan Wang, Yang Liu, Xuanjing Huang*

5. **Customized Image Narrative Generation via Interactive Visual Question Generation and Answering** CVPR, 2018. [paper](https://arxiv.org/pdf/1805.00460.pdf)
   
   *Andrew Shin, Yoshitaka Ushiku, Tatsuya Harada*

6. **Multimodal Differential Network for Visual Question Generation** EMNLP, 2018. [paper](https://www.aclweb.org/anthology/D18-1434.pdf)
   
   *Badri Narayana Patro, Sandeep Kumar, Vinod Kumar Kurmi, Vinay P. Namboodiri*

7. **A Question Type Driven Framework to Diversify Visual Question Generation** IJCAI, 2018. [paper](http://www.sdspeople.fudan.edu.cn/zywei/paper/fan-ijcai2018.pdf)
   
   *Zhihao Fan, Zhongyu Wei, Piji Li, Yanyan Lan, Xuanjing Huang*

8. **Visual Question Generation as Dual Task of Visual Question Answering.** CVPR, 2018. [paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Li_Visual_Question_Generation_CVPR_2018_paper.pdf)
   
   *Yikang Li, Nan Duan, Bolei Zhou, Xiao Chu, Wanli Ouyang, Xiaogang Wang, Ming Zhou* 

9. **Two can play this Game: Visual Dialog with Discriminative Question Generation and Answering.** CVPR, 2018. [paper](https://arxiv.org/pdf/1803.11186.pdf)
   
   *Unnat Jain, Svetlana Lazebnik, Alexander Schwing*

10. **Information Maximizing Visual Question Generation.** CVPR, 2019. [paper](https://arxiv.org/pdf/1903.11207.pdf)

   *Ranjay Krishna, Michael Bernstein, Li Fei-Fei*

11. **What Should I Ask? Using Conversationally Informative Rewards for Goal-oriented Visual Dialog.** ACL, 2019. [paper](https://www.aclweb.org/anthology/P19-1646.pdf)
   
   *Pushkar Shukla, Carlos Elmadjian, Richika Sharan, Vivek Kulkarni, Matthew Turk, William Yang Wang*

### [Distractor Generation](#distractor-generation)

Learning to generate distractors for multi-choice questions. 

1. **Generating Questions and Multiple-Choice Answers using Semantic Analysis of Texts.** COLING, 2016. [paper](https://www.aclweb.org/anthology/C16-1107.pdf)

   *Jun Araki, Dheeraj Rajagopal, Sreecharan Sankaranarayanan, Susan Holm, Yukari Yamakawa, Teruko Mitamura*

2. **Distractor Generation for Multiple Choice Questions Using Learning to Rank.** NAACL Workshop, 2018. [paper](https://www.aclweb.org/anthology/W18-0533.pdf) [code](https://github.com/harrylclc/LTR-DG)

   *Chen Liang, Xiao Yang, Neisarg Dave, Drew Wham, Bart Pursel, C. Lee Giles*

3. **Generating Distractors for Reading Comprehension Questions from Real Examinations.** AAAI, 2019. [paper](https://arxiv.org/pdf/1809.02768.pdf)

   *Yifan Gao, Lidong Bing, Piji Li, Irwin King, Michael R. Lyu*

### [Cross-lingual QG](#cross-lingual-QG)

Building cross-lingual models to generate questions in low-resource languages. 

1. **Cross-Lingual Training for Automatic Question Generation.** ACL, 2019. [paper](https://arxiv.org/pdf/1906.02525.pdf) [dataset](https://www.cse.iitb.ac.in/~ganesh/HiQuAD/clqg/)
   
   *Vishwajeet Kumar, Nitish Joshi, Arijit Mukherjee, Ganesh Ramakrishnan, Preethi Jyothi*

2. **Cross-Lingual Natural Language Generation via Pre-Training.** AAAI, 2020. [paper](https://arxiv.org/pdf/1909.10481.pdf)

   *Zewen Chi, Li Dong, Furu Wei, Wenhui Wang, Xian-Ling Mao, Heyan Huang*


## [Evaluation](#evaluation)

This direction investigates the mechanism behind question asking, and how to evaluate the quality of generated questions. 

1. **Question Asking as Program Generation.** NeurIPS, 2017. [paper](https://arxiv.org/pdf/1711.06351.pdf)
   
   *Anselm Rothe, Brenden M. Lake, Todd M. Gureckis.*

2. **Towards a Better Metric for Evaluating Question Generation Systems.** EMNLP, 2018. [paper](https://www.aclweb.org/anthology/D18-1429/)
   
   *Preksha Nema, Mitesh M. Khapra.*

3. **Evaluating Rewards for Question Generation Models.** NAACL, 2019. [paper](https://arxiv.org/pdf/1902.11049.pdf)
   
   *Tom Hosking and Sebastian Riedel.*

## [Resources](#resources)

QG-specific datasets and toolkits. 

1. **LearningQ: A Large-Scale Dataset for Educational Question Generation.** ICWSM, 2018. [paper](https://yangjiera.github.io/works/icwsm2018.pdf)
   
   *Guanliang Chen, Jie Yang, Claudia Hauff, Geert-Jan Houben.*

2. **ParaQG: A System for Generating Questions and Answers from Paragraphs.** EMNLP Demo, 2019. [paper](https://arxiv.org/pdf/1909.01642.pdf)
   
   *Vishwajeet Kumar, Sivaanandh Muneeswaran, Ganesh Ramakrishnan, Yuan-Fang Li.*

3. **How to Ask Better Questions? A Large-Scale Multi-Domain Dataset for Rewriting Ill-Formed Questions.** AAAI, 2020. [paper](https://arxiv.org/pdf/1911.09247.pdf) [code](https://github.com/ZeweiChu/MQR)
   
   *Zewei Chu, Mingda Chen, Jing Chen, Miaosen Wang, Kevin Gimpel, Manaal Faruqui, Xiance Si.*



