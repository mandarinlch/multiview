# Multi-view Spectral Clustering Network(MvSCN)
- 使用The v-th SiameseNet，通过一个和正负样本对相关的目标函数进行优化
- 利用SiameseNet学习到的表示构建亲和矩阵
- 使用神经网络对不同view的的X进行embeding，然后根据view内相似性（包含亲和矩阵）和view间一致性loss进行优化
- 随后是一个正交层，以将节点特征映射到正交空间
- 最后将特征concat起来，使用k-means得到最终结果
