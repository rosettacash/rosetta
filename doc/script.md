比特币脚本需要是一种功能谓语系统，当节点接收到新的交易时，首先，要获取所需的信息，然后运行脚本，主栈返回为True则代表交易的
输入是合法的。

我们需要实现一个OpCodes的解释器模块，有一个eval/1函数，输入是binary形式的脚本，输出是两个栈的最后结果。