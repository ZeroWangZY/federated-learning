# 联邦学习 Federated Learning

[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE) [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu) 


Everything about federated learning. *Your contribution is highly valued!* 

关于联邦学习的资料，包括：介绍、综述文章、最新文章、代表工作及其代码、数据集、论文等等。 *欢迎一起贡献！* 

---

- 目录
    - [1. 教程 Tutorial](#1-教程-Tutorial)
    - [2. 相关论文 Related Papers](#2-相关论文-Related-Papers)
    - [3. 项目 Project](#3-项目-Project)
    - [4. 相关学者 Related Scholars](#4-相关学者-Related-Scholars)

---

## 1. 教程 Tutorial

- 文字
    - [杨强：联邦学习](https://mp.weixin.qq.com/s/5FTrG5SZey2yeIbuyT3HoQ)
    - [Google - Federated Learning: Collaborative Machine Learning without Centralized Training Data](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html)
    - [联邦学习的研究及应用](https://mp.weixin.qq.com/s?src=11&timestamp=1555896266&ver=1561&signature=ZtLlc7qakNAdw8hV3dxaB30PxtK9hAshYsIxccFf-D4eJrUw6YKQcqD0lD3SDMEn4egQTafUZr429er7SueP6HKLTr*uFKfr6JuHc3OvfdJ-uExiEJStHFynC65htbLp&new=1)
    - [杨强：GDPR对AI的挑战和基于联邦迁移学习的对策](https://zhuanlan.zhihu.com/p/42646278) 

- PPT
    - [联邦学习的研究与应用](https://aisp-1251170195.file.myqcloud.com/fedweb/1553845987342.pdf)
    - [Federated Learning and Transfer Learning for Privacy, Security and Confidentiality](https://aisp-1251170195.file.myqcloud.com/fedweb/1552916850679.pdf) (AAAI-19)
    - [GDPR, Data Shortage and AI](https://aisp-1251170195.file.myqcloud.com/fedweb/1552916659436.pdf) (AAAI-19) 

- 视频
    - [GDPR, Data Shortage and AI](https://aaai.org/Conferences/AAAI-19/invited-speakers/#yang) (AAAI-19 Invited Talk) 

- 新闻
    - 2019/02/09 [谷歌发布全球首个产品级移动端分布式机器学习系统，数千万手机同步训练](https://www.jiemian.com/article/2853096.html)

---

## 2. 相关论文 Related Papers

- 综述与介绍 Survey And Introduction
    - arXiv 201912 - [Advances and Open Problems in Federated Learning](https://arxiv.org/abs/1912.04977) 58位学者联名综述
    - TIST 201902 - [Federated Machine Learning: Concept and Applications](https://dl.acm.org/citation.cfm?id=3298981) 
    - arXiv 201909 - [Federated Learning in Mobile Edge Networks: A Comprehensive Survey](https://arxiv.org/abs/1909.11875)
- 应用 Application
    - 2019 - [Federated Learning for Mobile Keyboard Prediction](https://arxiv.org/abs/1811.03604) - Google将联邦学习用于自家输入法 
    - 2019 - [Towards Federated Learning at Scale: System Design](https://arxiv.org/abs/1902.01046) - Google千万设备级联邦学习系统设计
- 联邦学习的提出 
    - 2015 - [Federated Optimization:Distributed Optimization Beyond the Datacenter](https://arxiv.org/abs/1511.03575)
    - 2016 - [Practical Secure Aggregation for Federated Learning on User-Held Data](https://arxiv.org/abs/1611.04482)
    - 2016 - [Federated Optimization: Distributed Machine Learning for On-Device Intelligence](https://arxiv.org/abs/1610.02527)
    - 2017 - [Federated Learning: Strategies for Improving Communication Efficiency](https://arxiv.org/abs/1610.05492)
    - 2017 - [Communication-Efficient Learning of Deep Networks from Decentralized Data](https://arxiv.org/abs/1602.05629) 联邦平均算法 the FederatedAveraging algorithm
- 联邦学习安全性
    - NIPS 2016 - [Practical Secure Aggregation for Federated Learning on User-Held Data](https://arxiv.org/abs/1611.04482) 增强联邦学习的隐私保护能力
    - 2017 - [Differentially Private Federated Learning: A Client Level Perspective](https://arxiv.org/abs/1712.07557) 使用差分隐私避免泄露用户的贡献度
    - 2018 - [How to Backdoor Federated Leraning](https://arxiv.org/abs/1807.00459) Model Poisoning攻击
    - 2019 - [Can You Really Backdoor Federated Learning](https://arxiv.org/abs/1911.07963) 如何避免联邦学习被后门攻击
    - ICML 2019 - [Analyzing Federated Learning through an Adversarial Lens](https://arxiv.org/abs/1811.12470) Model Poisoning攻击
    - ICLR 2020 - [DBA: Distributed Backdoor Attacks against Federated Learning](https://openreview.net/forum?id=rkgyS0VFvr) Model Poisoning攻击，在两个最新鲁棒FL框架上验证
    - AAAI 2020 - [Robust Federated Training via Collaborative Machine Teaching using Trusted Instances](https://arxiv.org/abs/1905.02941) 鲁棒FL方法，诊断训练集中的Bugs和调整label.
- 联邦学习扩展(FL+)
    - NIPS 2017 - [Federated Multi-Task Learning](http://papers.nips.cc/paper/7029-federated-multi-task-learning) 联邦多任务学习
    - arXiv 201901 - [Federated Reinforcement Learning](https://arxiv.org/abs/1901.08277) 联邦学习 + 强化学习 (Federated Learning + Reinforcement Learning)
    - arXiv 201901 - [SecureBoost: A Lossless Federated Learning Framework](https://arxiv.org/abs/1901.08755) 纵向联邦学习 (Vertical Federated Learning) 使用分布式决策树 
    - arXiv 201810 - [Secure Federated Transfer Learning](https://arxiv.org/abs/1812.03337) 联邦迁移学习
    - ICML 2019 - [Bayesian Nonparametric Federated Learning of Neural Networks](https://arxiv.org/abs/1905.12022) 贝叶斯联邦学习
    - ICLR 2020 - [Federated Adversarial Domain Adaptation](https://arxiv.org/abs/1911.02054)  联邦对抗域适应
- 高效联邦学习
    - 2018 - [Expanding the Reach of Federated Leraning by Reducing Client Resource Requirements](https://arxiv.org/abs/1812.07210) 提出两个策略来提高通信效率
    - 2019 - [Robust and Communication-Efficient Federated Learning from Non-IID Data](https://arxiv.org/abs/1903.02891) 提出压缩框架STC，可以减少训练时间和通信代价

---

## 3. 项目 Project

- [FATE - 微众银行](https://github.com/WeBankFinTech/FATE)
- [TensorFlow Federated](https://github.com/tensorflow/federated)
- [Federated-Learning](https://github.com/roxanneluo/Federated-Learning) : An implement of google's paper.

---

## 4. 相关学者 Related Scholars

- [杨强 Yang Qiang](https://scholar.google.com/citations?hl=en&user=1LxWZLQAAAAJ)
- [H. Brendan McMahan](https://scholar.google.com/citations?user=iKPWydkAAAAJ&hl=en)
- [jakub konečný](https://scholar.google.com/citations?user=4vq7eXQAAAAJ&hl=en)

---

## 欢迎参与贡献