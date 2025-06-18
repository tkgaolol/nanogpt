notes:

1. 残差是指你将你原始输出 除了直接输入到下一层 还可以直接输入到在下一层<br>
    a. 这样可以加速推理， 因为顶部流出的梯度（顶部是指最终输出端）他会均匀地分配给他底下的分支
    即从顶部流出的梯度通过残差路径可以直接流向输入

2. attentions is a communication operation<br>
    a. aggregation function<br>
    b. pooling function<br>
    c. weighted sum function<br>
    d. reduce operation

3. torch.compile 可以让你的模型先编译一遍让系统知道你待会儿要干啥 而不用每一步每一个forward他都重新load东西进去


 

