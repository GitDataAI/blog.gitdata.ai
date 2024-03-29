---
slug: AndrewNG-DCAI
title: 【翻译】吴恩达:是时候采用DCAI了！
authors: taoshengshi
tags: [DCAI, 原则]
---

# 【翻译】是时候采用DCAI了！
这位人工智能先驱表示，现在是时候为大问题提供智能规模的、“以数据为中心”的解决方案了！

原文：  
Andrew Ng: Unbiggen AI - IEEE Spectrum
https://spectrum.ieee.org/andrew-ng-data-centric-ai

吴恩达在人工智能领域颇有声望。2000年代末，他与斯坦福大学的学生一起率先使用图形处理单元(gpu)来训练深度学习模型，并于2011年共同创立了谷歌大脑(Google Brain)，随后在百度担任了三年首席科学家，帮助这家中国科技巨头建立了人工智能团队。因此，当他说他已经确定了人工智能的下一个重大转变时，人们会倾听。这是他在IEEE Spectrum的独家问答中告诉我们的。

吴恩达目前的工作重点是他的公司Landing AI，该公司建立了一个名为LandingLens的平台，帮助制造商利用计算机视觉改进视觉检测。他还成为了他所谓的以数据为中心的人工智能运动的传播者，他说这可以为人工智能的大问题提供“小数据”解决方案，包括模型效率、准确性和偏见。

Andrew Ng谈……

* 大模型的下一步是什么
* 他不听的职业建议
* 定义以数据为中心的AI运动
* 合成数据
* 为什么Landing AI要求它的客户做这项工作

在过去十年左右的时间里，深度学习的巨大进步是由越来越大的模型处理越来越多的数据推动的。一些人认为这是一个不可持续的轨迹。你同意不能再这样下去了吗?

吴恩达:这是个大问题。我们已经在NLP(自然语言处理)中看到了基础模型。我对NLP模型变得更大，以及在计算机视觉中建立基础模型的潜力感到兴奋。我认为视频领域还有很多有待开发的领域:由于计算带宽和处理视频的成本，我们还没有能够为视频建立基础模型，而不是标记化文本。所以我认为这个扩展深度学习算法的引擎，已经运行了大约15年了，仍然有动力。话虽如此，它只适用于某些问题，还有一系列其他问题需要小数据解决方案。

当你说你想要一个计算机视觉的基础模型时，你是什么意思?

吴恩达:这是Percy Liang和我在斯坦福大学的一些朋友创造的一个术语，指的是在非常大的数据集上训练的非常大的模型，可以针对特定的应用进行调整。例如，GPT-3就是[NLP]基础模型的一个例子。基础模型作为开发机器学习应用程序的新范式提供了很多希望，但在确保它们合理公平和没有偏见方面也存在挑战，特别是如果我们中的许多人将在它们的基础上进行构建。

要建立一个视频的基础模型，需要发生什么?

吴恩达:我认为这是一个可扩展性问题。处理大量视频图像所需的计算能力非常重要，我认为这就是为什么基础模型首先在NLP中出现的原因。许多研究人员都在研究这个问题，我认为我们已经看到了计算机视觉领域开发这种模型的早期迹象。但我相信，如果半导体制造商给我们10倍的处理器能力，我们可以很容易地找到10倍的视频来建立这样的视觉模型。

话虽如此，过去十年发生的很多事情是，深度学习发生在面向消费者的公司中，这些公司拥有庞大的用户基础，有时是数十亿用户，因此拥有非常大的数据集。虽然这种机器学习模式已经为消费软件带来了很多经济价值，但我发现这种规模配方并不适用于其他行业。


听你这么说很有趣，因为你早期的工作是在一家拥有数百万用户的面向消费者的公司。

吴恩达:十多年前，当我提议启动谷歌大脑项目，使用谷歌的计算基础设施来构建非常大的神经网络时，这是一个有争议的步骤。一位非常资深的人把我拉到一边，警告我，创办谷歌大脑会对我的职业生涯不利。我想他觉得这个行动不能只是扩大规模，而我应该专注于架构创新。

> “在许多根本不存在庞大数据集的行业中，我认为重点必须从大数据转向优质数据。只要有50个精心设计的例子，就足以向神经网络解释你想让它学习什么。”
——Landing AI首席执行官兼创始人吴恩达

我记得当我和我的学生发表了第一篇NeurIPS研讨会论文，提倡使用CUDA(一种基于gpu的处理平台)进行深度学习时，一位AI领域的资深人士坐下来对我说:“CUDA编程真的很复杂。作为一种编程范例，这似乎工作量太大了。”我的确设法说服了他;另一个我没有说服的人。

我想他们现在都被说服了。

吴恩达:我想是的。

在过去的一年里，当我和人们谈论以数据为中心的人工智能运动时，我想起了10年或15年前我和人们谈论深度学习和可扩展性时的情景。在过去的一年里，我一直听到“这里没有什么新东西”和“这似乎是错误的方向”。

你如何定义以数据为中心的人工智能，为什么你认为这是一场运动?

吴恩达:以数据为中心的人工智能是系统地设计成功构建人工智能系统所需的数据的学科。对于一个人工智能系统，你必须用代码实现一些算法，比如一个神经网络，然后在你的数据集上训练它。过去十年的主流模式是下载数据集，同时专注于改进代码。由于这种模式，在过去的十年中，深度学习网络有了显著的改进，对于许多应用程序来说，代码——神经网络架构——基本上是一个解决的问题。因此，对于许多实际应用来说，现在更有效的方法是固定神经网络架构，而不是寻找改进数据的方法。

当我开始讲这个的时候，有很多从业者，完全恰当地，举起他们的手说:“是的，我们已经做这个20年了。”现在是时候把一些人凭直觉做的事情变成一个系统的工程学科了。

以数据为中心的人工智能运动远不止一家公司或一组研究人员。我和我的合作者在NeurIPS组织了一个以数据为中心的人工智能研讨会，我真的很高兴有这么多的作者和演讲者出席。

您经常谈到只有少量数据可供使用的公司或机构。以数据为中心的人工智能如何帮助他们?

吴恩达:你听过很多关于用数百万张图片构建视觉系统的说法——我曾经用3.5亿张图片构建了一个人脸识别系统。为数以亿计的图像构建的架构不能仅用于50个图像。但事实证明，如果你有50个真正好的例子，你可以建立一些有价值的东西，比如缺陷检查系统。在许多根本不存在庞大数据集的行业中，我认为重点必须从大数据转向好数据。有50个精心设计的例子就足以向神经网络解释你想让它学习什么。

当你说训练一个只有50张图片的模型时，这真的意味着你是在使用一个现有的模型，这个模型是在一个非常大的数据集上训练的，并且对它进行微调吗?或者你指的是一个全新的模型，它被设计成只从那个小数据集中学习?

吴恩达:让我来描述一下Landing AI的功能。在为厂家做目视检查时，我们经常使用我们自己的口味的RetinaNet。这是一个预训练的模型。话虽如此，预训练只是拼图的一小部分。更大的难题是提供工具，使制造商能够选择正确的图像集(用于微调)，并以一致的方式标记它们。有一个非常实际的问题，我们已经看到跨越视觉，NLP和语音，即使是人类注释者也不同意适当的标签。对于大数据应用，常见的反应是:如果数据是有噪声的，那么我们就获取大量数据，然后算法对其进行平均。但是，如果您可以开发工具来标记数据不一致的地方，并为您提供一种非常有针对性的方法来改善数据的一致性，那么这将是获得高性能系统的更有效方法。

> “收集更多数据通常会有所帮助，但如果你试图为所有事情收集更多数据，那可能是一项非常昂贵的活动。” ——Landing AI首席执行官兼创始人吴恩达

例如，如果你有1万张图片，其中30张图片属于一个类别，这30张图片的标签不一致，我们要做的一件事就是建立工具，把你的注意力吸引到不一致的数据子集上。因此，你可以很快地重新标记这些图像，使其更加一致，这将导致性能的提高。

这种对高质量数据的关注是否有助于消除数据集的偏差?如果你能在训练前对数据进行更多的整理?

吴恩达:确实如此。许多研究人员指出，有偏见的数据是导致有偏见系统的众多因素之一。为了设计这些数据，人们做了很多深思熟虑的努力。在NeurIPS研讨会上，Olga Russakovsky对此做了一个很好的演讲。在NeurIPS的主要会议上，我也非常喜欢Mary Gray的演讲，她谈到了以数据为中心的AI是解决方案的一部分，但不是整个解决方案。像datassheets for Datasets这样的新工具似乎也是这个难题的重要组成部分。

以数据为中心的人工智能提供给我们的强大工具之一是设计数据子集的能力。想象一下，训练一个机器学习系统，发现它的性能对大多数数据集都是可以的，但它的性能只对一小部分数据有偏差。如果你试图改变整个神经网络架构来提高这个子集的性能，这是相当困难的。但如果你能设计数据的一个子集，你就能以一种更有针对性的方式解决问题。

当你谈到数据工程时，你的确切意思是什么?

吴恩达:在人工智能中，数据清理很重要，但数据清理的方式通常是非常手动的。在计算机视觉中，有人可能会通过Jupyter笔记本可视化图像，可能会发现问题，可能会修复它。但我对那些能让你拥有一个非常大的数据集的工具感到兴奋，这些工具能快速有效地把你的注意力吸引到数据子集上，比如标签是嘈杂的。或者快速将您的注意力转移到100个类中的一个类上，收集更多的数据将使您受益。收集更多的数据通常会有所帮助，但如果您试图为所有事情收集更多的数据，那么这可能是一项非常昂贵的活动。

例如，我曾经发现，当背景中有汽车噪音时，语音识别系统的表现很差。知道了这一点，我可以在汽车噪音的背景下收集更多的数据，而不是试图为所有事情收集更多的数据，这将是昂贵和缓慢的。

使用合成数据怎么样，这通常是一个好的解决方案吗?

吴恩达:我认为合成数据是以数据为中心的人工智能工具箱中的一个重要工具。在NeurIPS研讨会上，Anima Anandkumar做了一个关于合成数据的精彩演讲。我认为合成数据的重要用途不仅仅是作为增加学习算法数据集的预处理步骤。我希望看到更多的工具让开发人员使用合成数据生成作为迭代机器学习开发闭环的一部分。

你的意思是合成数据可以让你在更多的数据集上尝试这个模型吗?

吴恩达:不完全是。这里有一个例子。假设你正在尝试检测智能手机外壳的缺陷。智能手机上有许多不同类型的缺陷。可能是划痕，凹痕，凹痕，材料变色，其他类型的污点。如果你训练模型，然后通过错误分析发现它总体上做得很好，但在凹痕上表现不佳，那么合成数据生成可以让你以更有针对性的方式解决问题。您可以仅为坑标记类别生成更多数据。

> “在消费软件互联网上，我们可以训练少量的机器学习模型来服务10亿用户。在制造业，你可能有1万家制造商打造1万个定制的人工智能模型。” ——Landing AI首席执行官兼创始人吴恩达

合成数据生成是一个非常强大的工具，但我通常会先尝试许多更简单的工具。比如数据增强，提高标签一致性，或者只是要求工厂收集更多的数据。

为了使这些问题更具体，你能给我举个例子吗?当一家公司找到Landing AI并说它在视觉检查方面存在问题时，你如何让它们进入并努力部署?

吴恩达:当客户来找我们时，我们通常会和他们谈谈他们的检查问题，然后看一些图像来验证这个问题在计算机视觉上是可行的。假设是，我们要求他们将数据上传到LandingLens平台。我们经常就以数据为中心的人工智能方法向他们提供建议，并帮助他们标记数据。

Landing AI的重点之一是让制造企业自己完成机器学习工作。我们的很多工作都是为了确保软件快速易用。通过机器学习开发的迭代过程，我们建议客户如何在平台上训练模型，何时以及如何改进数据的标记，从而提高模型的性能。我们的培训和软件通过将训练过的模型部署到工厂的边缘设备来支持他们。

你如何应对不断变化的需求?如果工厂的产品或照明条件发生变化，模型能跟上吗?

吴恩达:这因制造商而异。在许多情况下都存在数据漂移。但有些制造商已经在同一条生产线上运行了20年，几乎没有什么变化，所以他们不希望未来5年发生变化。那些稳定的环境使事情变得更容易。对于其他制造商，我们提供了工具来标记出现严重的数据漂移问题。我发现赋予制造业客户纠正数据、重新培训和更新模型的能力非常重要。因为如果有什么变化，现在是美国的凌晨3点，我希望他们能够立即调整他们的学习算法来维持运营。

在消费软件互联网上，我们可以训练少量的机器学习模型来服务10亿用户。在制造业，你可能有1万家制造商构建1万个定制的人工智能模型。挑战在于，如何在不需要雇佣1万名机器学习专家的情况下做到这一点?

所以你是说要扩大规模，你必须授权客户去做很多培训和其他工作。

吴恩达:没错!这是人工智能行业的一个全行业问题，而不仅仅是制造业。看看医疗保健。每家医院的电子健康记录格式都略有不同。每家医院如何训练自己的定制人工智能模型?期望每个医院的IT人员都发明新的神经网络架构是不现实的。摆脱这种困境的唯一方法是构建工具，通过为客户提供设计数据和表达其领域知识的工具，使他们能够构建自己的模型。这就是Landing AI在计算机视觉领域所执行的任务，而AI领域需要其他团队在其他领域执行这一任务。

你认为对于人们理解你正在做的工作或以数据为中心的人工智能运动，还有其他重要的事情吗?

吴恩达:在过去的十年里，人工智能最大的转变是向深度学习的转变。我认为，在这十年中，最大的转变很可能是向以数据为中心的人工智能转变。随着当今神经网络架构的成熟，我认为对于许多实际应用来说，瓶颈将是我们是否能够有效地获得开发工作良好的系统所需的数据。以数据为中心的人工智能运动在整个社区具有巨大的能量和势头。我希望更多的研究人员和开发人员能参与进来，为之努力。