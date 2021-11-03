# LSTM

本项目在不使用Pytorch包装好的LSTM函数下，实现了在单层LSTM与双层LSTM。

## 文件介绍

LSTM.py文件为使用Pytorch内包装好的LSTM函数

LSTMLM.py文件为手动实现**<u>单层LSTM</u>**

doubleLSTMLM.py文件为手动实现**<u>双层LSTM</u>**

## 原理讲解

本项目针对LSTM核心单元使用的是Pytorch框架内提供的公式，具体如下图所示：

$$
\begin{array}{ll} \\
            i_t = \sigma(W_{ii} x_t + b_{ii} + W_{hi} h_{t-1} + b_{hi}) \\
            f_t = \sigma(W_{if} x_t + b_{if} + W_{hf} h_{t-1} + b_{hf}) \\
            g_t = \tanh(W_{ig} x_t + b_{ig} + W_{hg} h_{t-1} + b_{hg}) \\
            o_t = \sigma(W_{io} x_t + b_{io} + W_{ho} h_{t-1} + b_{ho}) \\
            c_t = f_t \odot c_{t-1} + i_t \odot g_t \\
            h_t = o_t \odot \tanh(c_t) \\
        \end{array}
$$

## 心得体会

通过本次项目，我巩固理解了LSTM的基本原理，并动手实现了单层与双层LSTM。同时借此机会，我学会了书写简单的Markdown文本以及github的简单实用。在本次课程中，我不仅学会了统计机器翻译的基本知识，同时也了解了当前机器翻译领域前沿的深度学习技术，开阔了我的视野，受益匪浅。

