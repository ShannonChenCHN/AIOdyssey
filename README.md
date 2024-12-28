# AI | Machine Learning | Deep Learning | NLP | LLM | ChatGPT

## 术语
AI、AIGC、AGI、token、LLM、大模型、GPT、ChatGPT、幻觉、AI agent、Prompt、Prompt Engineering、Function calling、Embedding、RAG、知识库、打标、标注、数据标注、标注数据（输入-输出对）、pair、召回、召回率、语义召回、向量(vector)、向量化、文本向量化、vector database、COT(Chain of Thought)、FSL(Few-Shot Learning)、Fine-tuning、SFT（Supervised Fine-Tuning，监督微调）、DPO 和 RLHF、模型训练、预训练、pre-training and post-training、模型压缩、量化（Quantization）、剪枝（Pruning）、知识蒸馏（Knowledge Distillation）、Model Distillation/Language Distillation（模型蒸馏）、推理优化（inference）、context window、泛化、泛化能力、拟合、过拟合、神经网络、超参、损失函数、自爆 AI、光谱、LoRA、scaling law、ground truth、[混入预置数据](https://www.volcengine.com/docs/82379/1221664#%E6%98%AF%E5%90%A6%E6%B7%B7%E5%85%A5%E9%A2%84%E7%BD%AE%E6%95%B0%E6%8D%AE)


## 知识体系
学习重点：LLM，fine-tuning  
学习目标：让 bot 学会某个人说话的风格  
学习方法：
- 带着目标和问题学习
- 多动手：practice, practice, practice
- 费曼学习法：包括写下来、写博客公众号、讲给别人听、做分享
- 《软件能》的“十步学习法”：https://time.geekbang.org/column/article/127656
- 学会利用 AI 工具(ChatGPT、Claude 等)辅助学习


学习计划


## 学习资料

### 必读（可以先扫一眼，快速浏览）🚀
- 李沐老师的GPT，GPT-2，GPT-3 论文精读视频：https://www.bilibili.com/video/BV1AF411b7xQ
   - 视频中提到的论文：
     - GPT-1: Improving Language Understanding by Generative Pre-Training: https://paperswithcode.com/paper/improving-language-understanding-by
     - GPT-2: Language Models are Unsupervised Multitask Learners: https://paperswithcode.com/paper/language-models-are-unsupervised-multitask
     - GPT-3: Language Models are Few-Shot Learners: https://arxiv.org/abs/2005.14165
- State of GPT by Andrej Karpathy (Microsoft Build 2023): https://www.youtube.com/watch?v=bZQun8Y4L2A&ab_channel=MicrosoftDeveloper
  - “这个是 GPT 官方分享训练过程，注意 PPT 里面的文字、表格信息量也非常大。试着暂停，然后去理解每一句话、每一个数字的含义。 ”
  - “Massively insightful talk by Andrej… He goes over how GPT is trained, gives some love to LLaMA, and offers some prompting tips. MUST WATCH!!!”
  - This video is one of many sessions delivered at the Microsoft Build 2023 event. | In this session, you will hear from Andrej Karpathy on the training pipeline of GPT assistants like ChatGPT, from tokenization to pretraining, supervised finetuning, and Reinforcement Learning from Human Feedback (RLHF). Dive deeper into practical techniques and mental models for the effective use of these models, including prompting strategies, finetuning, the rapidly growing ecosystem of tools, and their future extensions. | Andrej Karpathy is a Slovak-Canadian computer scientist who served as the director of artificial intelligence and Autopilot Vision at Tesla. He currently works for OpenAI, where he specializes in deep learning and computer vision.
- Instruct GPT: https://openai.com/research/instruction-following （最接近 GPT-3.5 的一篇论文）
- 斯坦福的人工智能小镇论文
   - 爆火论文打造《西部世界》雏形：25个AI智能体，在虚拟小镇自由成长：https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650873616&idx=1&sn=966d427ec1675f3a2c5f439d75f5ca65
     - 论文：https://arxiv.org/abs/2304.03442
   - 逼真到离谱！1000个人类「克隆」进西部世界，AI相似度85%细节太炸裂：https://mp.weixin.qq.com/s/FKLCKHhP7xgYArLISDdiaw
     - 论文：https://arxiv.org/abs/2411.10109
- 各大 LLM 官方文档（可以先扫一眼，快速浏览）
- 📖 《What Is ChatGPT Doing … and Why Does It Work?》(By Stephen Wolfram Writings)（微信读书上有中文版）: https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/
  - 🎬 What is ChatGPT doing...and why does it work? Wolfram：https://www.youtube.com/watch?v=flXrLGPY3SU&ab_channel=Wolfram
  - 🎬 How ChatGPT works | Stephen Wolfram and Lex Fridman https://www.youtube.com/watch?v=Ic88oVqr66w&ab_channel=LexClips
- 🎬 A Survey of Techniques for Maximizing LLM Performance: https://www.youtube.com/watch?v=ahnGLM-RC1Y&ab_channel=OpenAI
- Roadmap
   - 🎬 Advice for students by Andrej Karpathy: https://youtu.be/_au3yw46lcg?t=794&si=GLS7zZExauOu0nrk
   - 🎬 Advice for machine learning beginners | Andrej Karpathy and Lex Fridman: https://www.youtube.com/watch?v=I2ZK3ngNvvI&ab_channel=LexClips
   - 📖 How to Build Your Career in AI - by  Andrew Ng: https://info.deeplearning.ai/how-to-build-a-career-in-ai-book
   - 📃 AI Engineer Roadmap: https://roadmap.sh/ai-engineer
   - Greg Brockman: 我是如何成为一名机器学习实践者: https://mp.weixin.qq.com/s/nj2gUPdPYXVB3CfMh62EfA
-  书（可以先扫一眼，快速浏览）
   - 📖 《GPT 图解》(黄佳 著)
- 课程（可以先扫一眼，快速浏览）
   - WaytoAGI 推荐的课程合辑(左侧有分类)：https://waytoagi.feishu.cn/wiki/ZYtkwJQSJiLa5rkMF5scEN4Onhd?table=tblWqPFOvA24Jv6X&view=veweFm2l9w
   - https://www.deeplearning.ai/
- 非必读，但是有空的时候推荐阅读
   - 通向AGI之路：大型语言模型（LLM）技术精要: https://zhuanlan.zhihu.com/p/597586623


### 官方文档、资源
- OpenAI
  - [ ] OpenAI developer platform: https://platform.openai.com/docs/overview ⭐️⭐️⭐️
  - [ ] OpenAI Cookbook: https://cookbook.openai.com/ ⭐️⭐️⭐️
    - [ ] Related resources from around the web | OpenAI Cookbook https://cookbook.openai.com/articles/related_resources
  - OpenAI Dev-Day 2023: Breakout Sessions! https://community.openai.com/t/openai-dev-day-2023-breakout-sessions/505213
- Gemini
- Claude
  - 开发指南：https://docs.anthropic.com/en/home
  - Cookbook: https://github.com/anthropics/anthropic-cookbook
  - https://www.youtube.com/@anthropic-ai

 ### 书籍
 
技术原理类
- 《GPT 图解》(黄佳 著) ⭐️⭐️⭐️
- 《Python 自然语言处理》(Jalaj Thanaki 著) https://book.douban.com/subject/30350007/
- 《这就是 ChatGPT》(Stephen Wolfram 著) https://book.douban.com/subject/36449803/ ⭐️⭐️⭐️
  - 英文版：What Is ChatGPT Doing ... and Why Does It Work? https://book.douban.com/subject/36325029/
- 《ChatGPT原理与应用开发》https://book.douban.com/subject/36789967/ 
- 《大模型应用解决方案 : 基于GPT-3、ChatGPT、GPT-4等Transformer架构的自然语言处理》https://book.douban.com/subject/36696373/
- 《自然语言处理入门》(何晗 著) https://book.douban.com/subject/34856701/
- 《大模型应用开发极简入门》https://book.douban.com/subject/36764820/
- 《数学之美》(吴军 著) https://www.douban.com/doubanapp/dispatch?uri=/book/35033507 ⭐️⭐️⭐️

应用实践类
- 《ChatGPT营销实践》https://book.douban.com/subject/36954824/
- 《AI商业广告设计实战108招》https://book.douban.com/subject/36894358/
- 《AI绘画与摄影实战108招：ChatGPT+Midjourney+文心一格》https://book.douban.com/subject/36894373/
- 《AI短视频生成与剪辑实战108招：ChatGPT+剪映》https://book.douban.com/subject/36889464/
- 《ChatGPT+AI文案写作实战108招》https://book.douban.com/subject/36894218/
- 《智慧共生 ChatGPT与AIGC生产力工具实践》https://book.douban.com/subject/36427721/
- 《AI重塑演讲力：ChatGPT 10倍提升演讲写作与表达》https://book.douban.com/subject/36947415/

### 知识库
- [ ] 📃 通往 AGI 之路: https://waytoagi.feishu.cn/wiki/QPe5w5g7UisbEkkow8XcDmOpn8e ⭐️⭐️⭐️
- Generative AI Engineer 知識庫 - ihower's Notes https://ihower.tw/notes/generative-ai-engineer
- https://github.com/Hannibal046/Awesome-LLM


### 课程
- 入门课程推荐: https://waytoagi.feishu.cn/wiki/ZYtkwJQSJiLa5rkMF5scEN4Onhd?table=tblWqPFOvA24Jv6X&view=veweFm2l9w ⭐️⭐️⭐️
- 🎬 https://www.deeplearning.ai/ ⭐️⭐️⭐️⭐️⭐️
- Google AI Essentials: https://grow.google/ai-essentials/ ⭐️⭐️⭐️⭐️⭐️
- Machine Learning Crash Course | Google’s Engineering Education team: https://developers.google.com/machine-learning/crash-course ⭐️⭐️⭐️⭐️⭐️
- Five-day Gen AI Intensive live course created by Google and Kaggle: https://blog.google/technology/developers/google-kaggle-genai-intensive/
   - 5-Day Gen AI Intensive Course with Google Learn Guide| Kaggle: https://www.kaggle.com/learn-guide/5-day-genai#GenAI
- 🎬 YouTube Playlist
  - [ ] Understanding AI Models | by IBM Technology https://www.youtube.com/playlist?list=PLOspHqNVtKAC-FUNMq8qjYVw6_semZHw0
  - [ ] Large Language Models and Chatbots | by IBM Technology https://www.youtube.com/playlist?list=PLOspHqNVtKAAsiohuZj1Bt4XpA3_bkS3c
  - [ ] AI and Machine Learning with Google Cloud Tech | by Google Cloud Tech https://www.youtube.com/playlist?list=PLIivdWyY5sqJdmVMjLI8iCul14XkTRosn
  - 🎧 Large Language Models (LLMs) | by The TWIML AI Podcast with Sam Charrington https://www.youtube.com/playlist?list=PLILZm3MRkvH_Haw5riDiH3Eb1nNDauoox
  - Google’s AI Course for Beginners (in 10 minutes)! https://www.youtube.com/watch?v=Yq0QkCxoTHM&t=6s&ab_channel=JeffSu
  - Claude 3.5 Crash Course for Developers: Code 10x Faster in 2024 [Claude 3.5 artifacts] https://www.youtube.com/watch?v=fMa2zQIkQwM&ab_channel=codewithbrandon
- B 站
  - 李宏毅
  - 李沐

### 平台、工具
- https://huggingface.co/
- TABLUM’s LLM Explorer(开源LLM): https://llm.extractum.io/
- LLM 使用量排行：https://openrouter.ai/rankings/roleplay?view=week
- LMSYS 排行榜（人工）：https://lmarena.ai/?leaderboard

## 学习大纲
- [What is AI?](https://github.com/ShannonChenCHN/AIOdyssey/issues/1)
- [AI Learning Roadmap](https://github.com/ShannonChenCHN/AIOdyssey/issues/7)
- [Machine Learning](https://github.com/ShannonChenCHN/AIOdyssey/issues/2)
- [Deep Learning & Neural Network](https://github.com/ShannonChenCHN/AIOdyssey/issues/3)
- [NLP & LLM](https://github.com/ShannonChenCHN/AIOdyssey/issues/4)
- [LLMs: ChatGPT, Claude, Gemini...](https://github.com/ShannonChenCHN/AIOdyssey/issues/5)
- [AI Agent](https://github.com/ShannonChenCHN/AIOdyssey/issues/6)
- [Real-world Gen AI Use Cases](https://github.com/ShannonChenCHN/AIOdyssey/issues/8)
- [Get Hands Dirty & Build From Scratch](https://github.com/ShannonChenCHN/AIOdyssey/issues/9)
- [Build LLM-based Applications](https://github.com/ShannonChenCHN/AIOdyssey/issues/10)


### 同行分享交流
- 🎧 我在 Character.ai 做 Post Training｜对谈前 C.AI 模型应用算法专家 Ted | | 小宇宙 ⭐️⭐️⭐️: https://www.xiaoyuzhoufm.com/episode/67359e9843dc3a43878eaa90
- 🎧  #17 从通用走向个人，一个不同的大模型叙事——对话Me.bot创始人陶芳波 - 出海相对论 | 小宇宙 ⭐️: https://www.xiaoyuzhoufm.com/episode/66a20afd33ddcbb53c00e7ad
