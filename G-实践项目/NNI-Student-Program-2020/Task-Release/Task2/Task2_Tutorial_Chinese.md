# NNI 学生项目 2020：Task 2.2 任务指南

## 任务简介 ##

本个项目任务围绕超参调优（HPO）与神经网络架构搜索（NAS）开展，以 CIFAR-10 数据集为基础，通过训练深度学习模型，预测数据集标签。任务的难度系数从两星到五星不等，同学们可根据
自己的实际能力、学习情况与时间安排，选择适合自己的进阶之路。

如果您缺少相关项目经验或深度学习相关知识背景，建议您从步骤 0.1 开始。如果您已具备一定学习基础，可以从步骤 1 开始。其中，步骤 0.1 需要完成 Python 机器学习库 
Pytorch 入门训练；步骤 1 需要通过预定义的结构，训练深度学习模型；步骤 2 需要通过神经网络架构搜索，进一步训练和优化模型。

无论您是刚刚入门机器学习的小白，还是身经百战的“调参大师”，只要善于思考，乐于投入，每一位同学都能成为 NNI 的使用者乃至开发者。

准备好了吗？让我们和 NNI 一起开启全新的机器学习之旅吧！

## 步骤 0.1

Step 0.1 是热身环节，**PyTorch 文档**提供了详细的任务描述与操作流程，具体内容请[阅读文档](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)。

## 步骤 1

在步骤 1 中，您的主要任务是训练 `main.py`，您的目标很简单: 尽可能提升训练模型的准确率。

如果您仍然感到困惑，我将在这里给出一些提示。我们知道，如果直接运行 `main.py`  ，得到理想结果的可能性很低，寻找到最优的参数组合则是解决这一问题的关键。当您输入`python main.py -h`时，您将看到关于运行这段代码的众多选项，任务的关键在于，如何在这些选项中挑选最适合的参数组合?

如果您在这一过程中遇到困难，NNI 的超参调优功能（HPO）可以助您一臂之力。

关于 NNI **超参调优** (HPO) 的详细使用教程，请[阅读文档](https://nni.readthedocs.io/zh/latest/hyperparameter_tune.html)。

完成此步骤之后，您可以进一步了解本步骤中关于模型的其他细节，这将有助于您完成下一个任务。

## 步骤 2

在步骤 2 中，我们将尝试自主设计模型，更准确地说，是自动生成模型。正如`2-nas/model.py`所示，我们将从 DARTS 的搜索空间开始。

首先，您需要以步骤 1 训练得到的代码为基础，在搜索空间中选择随机结构，并验证性能。

然后，您可以通过使用 NNI 神经网络架构索功能（NAS），生成并优化模型。

关于**神经网络架构搜索** (NAS) 的详细使用教程，请[阅读文档](https://nni.readthedocs.io/zh/latest/nas.html)。


## 说明

关于使用 NNI 的详细教程，请访问 Github 社区：https://github.com/microsoft/nni

我们希望各个队伍独立完成任务，同时，也鼓励各位学员与导师积极沟通，及时反馈，这将有效推动您的项目。

期待大家的好消息！