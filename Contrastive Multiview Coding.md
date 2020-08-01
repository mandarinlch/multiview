## Contrastive Multiview Coding（CMC)
- 采用对比学习的思路，由view1、view2通过f1、f2得到z1、z2
- 利用正负样本对设计loss，其中，正样本对服从x ∼ p(v1, v2)或x = {vi1, vi2}，负样本对服从y ∼ p(v1)p(v2) 或 y = {vi1, vj2}。
  loss：以一个view为基准，正样本对的cos相似度大，负样本的cos相似度小。
- 采用 “full graph”和“core view”两种loss组合策略，使得不同view之间重复更多的属性被更多的考虑。
