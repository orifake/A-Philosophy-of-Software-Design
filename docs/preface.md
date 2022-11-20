---
id: preface
slug: /preface
sidebar_position: 2
---
# 前言
> Preface
> People have been writing programs for electronic computers for more than 80 years, but there has been surprisingly little conversation about how to design those programs or what good programs should look like. There has been considerable discussion about software development processes such as agile development and about development tools such as debuggers, version control systems, and test coverage tools. There has also been extensive analysis of programming techniques such as object-oriented programming and functional programming, and of design patterns and algorithms. All of these discussions have been valuable, but the core problem of software design is still largely untouched. David Parnas’ classic paper “On the Criteria to be used in Decomposing Systems into Modules” appeared in 1971, but the state of the art in software design has not progressed much beyond that paper in the ensuing 45 years.

80多年来，人们一直在通过电子计算机编写程序，但令人惊讶的是，很少有关于如何设计这些程序或好的程序应该是什么样子的讨论。关于软件开发流程例如敏捷开发，开发工具例如调试器，版本控制系统和测试覆盖率工具，已经有了相当多的讨论了。并且针对编程技术也已经有了广泛的研究，比如面向对象编程或者函数式编程，设计模式和算法。所有这些讨论都是有价值的，但是程序设计的核心问题很大程度上仍未被触及。David Parnas 的经典论文“关于将系统拆解成模块的标准”发表于 1971 年，但是在随后的 45 年里，软件设计的水平并这篇论文进步多少。

> The most fundamental problem in computer science is problem decomposition: how to take a complex problem and divide it up into pieces that can be solved independently. Problem decomposition is the central design task that programmers face every day, and yet, other than the work described here, I have not been able to identify a single class in any university where problem decomposition is a central topic. We teach for loops and object-oriented programming, but not software design.

计算机科学中最基本的问题是问题分解，如何处理复杂的问题将其分解为可以独立解决的部分。问题分解是程序员每天所面对的设计任务最核心的，但是除了这里描述的工作之外，我还没有在任何一所大学里找到一门以问题分解为中心的课程。我们讲授循环和面向对象的程序设计，而不是软件设计。

> In addition, there is a huge variation in quality and productivity among programmers, but we have made little attempt to understand what makes the best programmers so much better or to teach those skills in our classes. I have talked with several people I consider to be great programmers, but most of them had difficulty articulating specific techniques that give them their advantage. Many people assume that software design skill is an innate talent that cannot be taught. However, there is quite a bit of scientific evidence that outstanding performance in many fields is related more to high-quality practice than innate ability (see, for example, Talent is Overrated by Geoff Colvin).

此外，程序员之间在质量和生产率上存在巨大差异，但是我们几乎很少尝试去了解最好的程序员变好的原因，或者在我们的课堂上教授这些技能。我曾经与几位我认为最优秀的程序员交流，但是他们大多数人难以讲清哪些技术让他们变得更优秀。很多人都认为软件设计技能是与生俱来的天赋，难以被教授。但是，有许多科学研究证明很多领域的杰出表现更多地与高质量的实践有关，而不是天赋（例如，参见 Geoff Colvin 的《人才被高估》）

> For many years these issues have perplexed and frustrated me. I have wondered whether software design can be taught, and I have hypothesized that design skill is what separates great programmers from average ones. I finally decided that the only way to answer these questions was to attempt to teach a course on software design. The result is CS 190 at Stanford University. In this class I put forth a set of principles of software design. Students then work through a series of projects to assimilate and practice the principles. The class is taught in a fashion similar to a traditional English writing class. In an English class, students use an iterative process where they write a draft, get feedback, and then rewrite to make improvements. In CS 190, students develop a substantial piece of software from scratch. We then go through extensive code reviews to identify design problems, and students revise their projects to fix the problems. This allows students to see how their code can be improved by applying design principles.

多年来，这些问题让我困惑和沮丧。我开始疑惑软件设计是否能被教授，并且我开始假设软件设计技巧使优秀程序员脱颖而出。最终我觉得回答问题的唯一方式是尝试教授软件设计课程。之后斯坦福大学的 CS 190诞生了。在课中我提出了一系列的软件设计原则。学生们通过一系列的项目来吸收和时间这些原则。课程的授课方式类似于传统的英语写作课。在英语课堂上，学生使用迭代过程，在其中编写草稿，获得反馈，然后重写以进行改进。在 CS 190 中，学生从头开始开发了大量软件。然后，我们将进行了大量的代码审查来识别设计上的问题，之后学生修订项目解决问题。这使得学生们了解可以通过应用设计原理来改进其代码。

> I have now taught the software design class three times, and this book is based on the design principles that emerged from the class. The principles are fairly high level and border on the philosophical (“Define errors out of existence”), so it is hard for students to understand the ideas in the abstract. Students learn best by writing code, making mistakes, and then seeing how their mistakes and the subsequent fixes relate to the principles.

迄今为止，我已经教过3次软件设计课程，本书也是基于该课程中出现的设计原理编写的。这些原则是相当高的水平，并且近似于哲学（“定义不存在的错误”），因此学生很难理解这些较为抽象的思想。通过编写代码，犯错误，然后查看他们的错误以及后续通过相关的设计原则的修正这些错误，学生的学习取得了更好的效果。

> At this point you may well be wondering: what makes me think I know all the answers about software design? To be honest, I don’t. There were no classes on software design when I learned to program, and I never had a mentor to teach me design principles. At the time I learned to program, code reviews were virtually nonexistent. My ideas about software design come from personal experience writing and reading code. Over my career I have written about 250,000 lines of code in a variety of languages. I’ve worked on teams that created three operating systems from scratch, multiple file and storage systems, infrastructure tools such as debuggers, build systems, and GUI toolkits, a scripting language, and interactive editors for text, drawings, presentations, and integrated circuits. Along the way I’ve experienced firsthand the problems of large systems and experimented with various design techniques. In addition, I’ve read a considerable amount of code written by other people, which has exposed me to a variety of approaches, both good and bad.

你可能会非常疑惑一点：是什么让我认为我知道有关软件设计的所有答案？老实说，我没有。当我学会编程时，没有关于软件设计的课程，而且我从来没有导师来教我设计原理。在我学习编程时，也几乎没有代码审查。我对软件设计的想法完全来自于编写与阅读代码。在我的职业生涯中，我用多种语言编已经写了大约 250,000 行代码。我曾经在团队中工作过，这些团队从零开始创建了三个操作系统，多个文件和存储系统，基础结构工具（例如调试器，构建系统和 GUI 工具包），一门脚本语言以及用于文本，绘图，文稿演示和集成电路的交互式编辑器。在这过程中，我亲身经历了大型系统的问题，并尝试了各种设计技术。另外，我阅读了很多其他人编写的代码，这让我接触到了很多方法，无论是好是坏。

> Out of all of this experience, I’ve tried to extract common threads, both about mistakes to avoid and techniques to use. This book is a reflection of my experiences: every problem described here is one that I have experienced personally, and every suggested technique is one that I have used successfully in my own coding.

通过所有这些竟然，我尝试去获取通用的线索，包括应该避免的错误和应该使用的技巧。本书汇集了我的经验：这里描述的每个问题都是我亲身经历的，每种建议的技术都是我在自己的编码中所成功使用的。

> I don’t expect this book to be the final word on software design; I’m sure there are valuable techniques that I’ve missed, and some of my suggestions may turn out to be bad ideas in the long run. However, I hope that the book will start a conversation about software design. Compare the ideas in this book with your own experiences and decide for yourself whether the approaches described here really do reduce software complexity. This book is an opinion piece, so some readers will disagree with some of my suggestions. If you do disagree, try to understand why. I’m interested in hearing about things that work for you, things that don’t work, and any other ideas you may have about software design. I hope that the ensuing conversations will improve our collective understanding of software design. I will incorporate what I learn in future editions of this book.

我不希望这本书成为软件设计的定论。我很肯定，我错过了一些有价值的技术，从长远来看，我的一些建议可能会变成坏主意。但是，我希望本书能开启有关软件设计的讨论。将本书中的想法与您自己的经验进行比较，然后由你自己决定本书介绍的方法是否确实降低了软件复杂性。这本书是一篇观点文章，所以有些读者会不认同我的一些建议。如果你不认同，请尝试去理解其中的原因。我有兴趣了解对你有帮助的东西，或不起作用的东西以及任何你对软件设计的有其他想法。我会讲我所学到的添加到本书未来的修订版里。

> The best way to communicate with me about the book is to send email to the following address:

与我交流有关这本书的最好方法是将电子邮件发送到以下地址：
software-design-book@googlegroups.com

> I’m interested in hearing specific feedback about the book, such as bugs or suggestions for improvement, as well as general thoughts and experiences related to software design. I’m particularly interested in compelling examples that I can use in future editions of the book. The best examples illustrate an important design principle and are simple enough to explain in a paragraph or two. If you would like to see what other people are saying on the email address and participate in discussions, you can join the Google Group software-design-book.

我有兴趣听取有关本书的反馈，例如错误或改进建议，以及所有与软件设计相关的思想和经验。我对可以应用到本书未来版本的例子更为感兴趣。对于阐述一个重要设计原则的最好的例子，是足够简单可以在一个或两个篇章解释完。如果你希望阅读其他人在emal力说了什么并参与讨论的话，你可以加入Google Group software-design-book。
