# RAG




## 论文/文章研读

### RAFT: Adapting Language Model to Domain Specific RAG 

RAFT: Adapting Language Model to Domain Specific RAG 
- 论文链接：https://arxiv.org/abs/2403.10131
- GitHub：https://github.com/ShishirPatil/gorilla/tree/main/raft
- Berkeley Blog：https://gorilla.cs.berkeley.edu/blogs/9_raft.html
- Microsoft-Meta blog：https://techcommunity.microsoft.com/blog/aiplatformblog/raft-a-new-way-to-teach-llms-to-be-better-at-rag/4084674


#### Insights

1. 结合 RAG 进行 SFT 有助于提成 LLM 表现；
  - 怎么做呢？在训练时提供「问题 + context 信息+ CoT 答案」
  - 使用 Chain-of-Thought 的数据训练，能提升准确性，同时降低过拟合
2. 需要所有的训练数据都带上 context 信息吗？
  - 不需要，具体多少百分比，看具体的数据集
3. 在某些训练数据中提供一些干扰的 context 信息，提升模型的鲁棒性

#### Excerpts

![image](https://github.com/user-attachments/assets/2860806d-70bb-4550-9d13-68e126657d57)
![image](https://github.com/user-attachments/assets/81ca9db7-74f2-4c6c-9436-470c8e0bf094)


1. In this paper, 
  a. we present Retrieval Augmented Fine Tuning (RAFT), a training recipe which improves the model’s ability to answer questions in "open-book" in-domain settings.
  b. In training RAFT, given a question, and a set of retrieved documents, we train the model to ignore those documents that don’t help in answering the question, which we call, distractor documents. RAFT accomplishes this by citing verbatim the right sequence from the relevant document to help answer the question.
  c. This coupled with RAFT’s chain-of-thought-style response helps improve the model’s ability to reason

2. In this paper, we study how to combine instruction fine-tuning (IFT) with retrieval aug-
mented generation (RAG). 
  a. We propose a novel adaptation strategy – Retrieval-Augmented Fine Tuning (RAFT). 
  b. RAFT specifically addresses the challenge of fine-tuning LLMs to both incorporate domain knowledge while also improving in-domain RAG performance. 
  c. RAFT aims to not only enable models to learn domain-specific knowledge through fine-tuning, but also to ensure robustness against distracting retrieved information. This is achieved by training the models to understand the dynamics between the question (prompt), the domain-specific documents retrieved, and the right answer. Going back to our analogy to the open book exam, our approach is analogous to studying for an open-book exam by recognizing relevant, and irrelevant retrieved documents.

3. A key factor in enhancing training quality is the generation of a reasoning process, such as Chain-of-Thought, to explain the provided answers. RAFT approach is similar: we demonstrate that creating a full reasoning chain and in-addition, clearly citing sources enhances the model’s accuracy in answering questions. In Fig. 3, we illustrate this set-up. Generating the training data in this fashion, involves presenting the model with a question, context, and verified answers, and then requesting it to form a reasoning chain that appropriately references the original context.

   We demonstrate that adding detailed reasoning paragraphs can help boost the model’s performance in our experiment section.
   ![image](https://github.com/user-attachments/assets/d97c5224-7139-4ed6-a3f8-e8f57f6e2337)

4. Result: Using the above datasets and baselines, we evaluate our model RAFT and demonstrate the effectiveness of RAFT in Tab. 1. We see that RAFT consistently and significantly outperforms the baselines.  Compared with the base Llama-2 instruction-tuned model, RAFT with RAG does much better in terms of extracting information as well as being robust towards distractors.
  
   ![image](https://github.com/user-attachments/assets/84e3581b-94bf-4453-a8c3-b5554c3fef9d)

   By applying domain-specific tuning, we significantly enhance its performance. This process enables the model to learn and adopt the appropriate style of answering. However, introducing RAG to a domain-specifically fine-tuned (DSF) model doesn’t invariably lead to better outcomes. This might indicate that the model lacks training in context processing and extracting useful information from it. By incorporating our method, RAFT , we train the model not only to match its answering style with that required but also to improve its document processing capabilities. Consequently, our approach outperforms all others.
  
5. Effect of CoT

   ![image](https://github.com/user-attachments/assets/91b2b821-b800-4f37-b628-4bebebac5170)
   ![image](https://github.com/user-attachments/assets/a5b61f9d-34c1-4df0-aec8-df9ed41e2781)

6. Should we train the LLM always with the golden context for RAG?

   Our findings suggest that, for domain-specific RAG tasks, including a certain percentage of training data without the golden documents in the context proves to be advantageous.
   ![image](https://github.com/user-attachments/assets/ddfbf4bd-7f04-4702-83dc-6888371fa7b4)
   ![image](https://github.com/user-attachments/assets/0a6ddd1c-e286-4959-ae69-011e98ee1537)

7. Making Model Robust to top-K RAG

   ![image](https://github.com/user-attachments/assets/4070d46e-83cb-400f-b64e-1bac268e4032)
   ![image](https://github.com/user-attachments/assets/306135ab-e875-4bc2-a278-0bc4567e83a1)
   ![image](https://github.com/user-attachments/assets/ee170121-6543-4255-b412-68a06879048e)





