# KnowLogic 
The official repository of the KnowLogic Benchmark 📊  

🔗 **Hugging Face Dataset:** [KnowLogic on Hugging Face 🤗](https://huggingface.co/datasets/Pokerwf/KnowLogic)  
📄 **Paper:** [KnowLogic: A Knowledge-Driven Benchmark for Logical Reasoning](https://arxiv.org/pdf/2503.06218)  


## Timeline 🗓️  
- **2025.3.10**: We published our paper! 📄  
- **2025.3.11**: We released the dataset! 🎉  
- **Coming Soon**: Our evaluation code will be released! 🚀  

---

## Dynamic Data Synthesis 🛠️  

Our benchmark **KnowLogic** is generated through a knowledge-driven synthetic data strategy, which integrates diverse commonsense knowledge, plausible scenarios, and various types of logical reasoning. One of the key advantages of KnowLogic is its adjustable difficulty levels, allowing for flexible control over question complexity. It also includes fine-grained labels for in-depth evaluation of LLMs' reasoning abilities across multiple dimensions. Our benchmark consists of 3,000 bilingual (Chinese and English) questions across various domains. 🌍  

![Dynamic Data Synthesis](https://github.com/pokerwf/KnowLogic/blob/main/image/Overall.jpg)   

---

### **Step 1: Scenario Definition** 📝  
Select entities/events from the knowledge base, integrate them into a scenario framework, and generate introductory text using natural language templates. 🧩  

### **Step 2: Inference Data Generation** 🔍  
Use a Reasoner to expand initial facts, create a fact base with detailed features. The Reasoner verifies and adds facts until each entity/event's position is uniquely determined. ✅  

### **Step 3: Question Design** ❓  
The Question Generator takes the fact set and the ground-truth arrangement of entities/events as input to produce various question types. 🎯  

---

## Overall Evaluation on Different Models 📊  
![Overall Evaluation on Different Models](https://github.com/pokerwf/KnowLogic/blob/main/image/evaluation.jpg)   

Among the models tested, O1-Preview achieves the highest performance. 🥇 In contrast, DeepSeek-R1, the top-performing open-source model, underperforms relative to the closed-source models. Overall, our benchmark remains a challenging test, effectively highlighting the limitations of current models across various domains. Notably, LLMs specifically trained for inference tend to outperform general LLMs within the same family when tackling such complex questions. 🤔  

---

## Knowledge Entries 📚  
Knowledge entries written by human in four knowledge bases. The $X$ and $Y$ in the entry are placeholders for entities that can be filled in. The $A$ and $B$ are for events. The $T$ is for the times. The $V$ is for the value of natural properties. 🌟  

![Knowledge Entries](https://github.com/pokerwf/KnowLogic/blob/main/image/knowledge_entity.jpg)   

--- 

## 📑 Citation  
If you find **KnowLogic** useful in your research, we would appreciate it if you cite our paper:  

```bibtex
@article{zhan2025knowlogicbenchmarkcommonsensereasoning,
      title={KnowLogic: A Benchmark for Commonsense Reasoning via Knowledge-Driven Data Synthesis}, 
      author={Weidong Zhan and Yue Wang and Nan Hu and Liming Xiao and Jingyuan Ma and Yuhang Qin and Zheng Li and Yixin Yang and Sirui Deng and Jinkun Ding and Wenhan Ma and Rui Li and Weilin Luo and Qun Liu and Zhifang Sui},
      year={2025},
      eprint={2503.06218},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2503.06218}, 
}
