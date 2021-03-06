## 第一课作业

经过了连续几天的折腾，终于走到了交第一课总结作业的地步，感觉好不容易。下面我以一个小白的理解，来叙述一下第一课的感悟。


### 一、运用类比

课程一开始，老师并没有着急直接讲专业的编程知识，而是讲了一个银行开户的例子，从一张最简单的开户流程图开始，几经优化，勾勒出一幅效率更高的开户流程图。但是这绝对不是单纯的讲故事。

这一类比的方法，是为了形象的勾画出代码的一个运行流程图。客户最初提供的的表单就是一页代码。客户开卡，就是代码的输出结果。

这一页代码（开户申请单）经过内置库（内置服务），然后流转到编译器、解析器（银行的业务核心），经过编译器、解析器的执行，最终输出结果（客户开卡）。

真的很佩服老师的智谋，通过这么一个形象的类比，来阐述代码运行流程。这种类比确实非常有效。

今天我又看了一遍课程回放，对老师经常讲的一句话有了初步理解。这句话是：“编程最重要不是敲代码，而是思考。”  我的理解就是，如果不去优化银行的整个业务架构，仅仅是靠提高窗口人员的技术水平， 那么就是把窗口人员累死，恐怕银行的整体运营效率也提高不了多少，开户的人一多，银行系统就要崩溃。

反之，经过优化了银行的业务架构，也就是优化了环境框架，可以迅速提高运行效率，这个是本质的提高。



### 二、环境

提高环境，我就想起一个词，叫大环境。 老师通过类比讲故事的方法，是为了更好的阐释“编程语言的运行环境”。后来又举例婴儿、与小学生的生活环境，来类比程序的运行环境。简而言之，就是程序运行，到底需要多少组件类支撑他？ 他才能生存下去，也就是运行下去。

银行的运行环境，包括很多。内置服务（第三方服务），预处理服务，核心执行服务，等。
通过类比，代码的运行环境，也是雷同。包括内置库（第三方库），编译器/解析器，等。
只不过，不同的代码，不同的编程语言，他们需要的内置服务（内置库），是不相同的。但是代码整个运行的流程大致相同。


### 三、V8引擎：

V8引擎，通俗的讲就是8缸的发动机，缸体呈V字型排列。 在编程体系里面也有这个词汇，我去百度去搜，大概意思是：V8将其编译成原生机器码（IA-32, x86-64, ARM, or MIPS CPUs），并且使用了如内联缓存（inline caching）等方法来提高性能。有了这些功能，JavaScript程序在V8引擎下的运行速度媲美二进制程序。

请恕我水平太低，连读三遍，愣是没读懂。不过既然是引擎，那他肯定就是核心部件，有了它，整个运行环境才能运转下去。相较于银行的运行环境，V8引擎指的银行的就是银行的业务核心。这个核心部件，包括编译器/解析器，靠他们来执行。

至于V8引擎他们的原理，暂且不懂，不过V8发动机虽然不知道怎么制造的，但是只要能把车子开好，也OK。


### 四、编译器/解释（执行）器：

编译器/解析（执行）器，这个到底是两个机器呢，还是一个机器呢？ 

在编译型语言中，比如c语言，他就是两个机器，先编译，后解析执行。 银行开户时，预处理人员搞好后，在交给核心审核人员，最后输出。  这两个人分开干活，运行效率高，但是开发效率低。
在解析性语言，比如JS语言中，他就是同一台机器，边解析，边执行。银行开户时，预处理与核心审核，两个活都是这一个人干，运行效率低，开发效率高。

### 五、内置库：

内置库，这个在银行的运行环境中，就是指的内置服务。为了能够提高核心人员的运行效率，需要把客户的单子，进行同一的编排，嵌入，复印、格式化等。 
这个内置库，在语言运行环境中，就是给代码进行相关的包装、整形、打磨、切割、清洗、编码、统一格式、等，然后让代码能够高效率的通过V8引擎，快速输出。或者说是为了让V8引擎快速识别他，并处理他，执行他。

### 六、第三方库：

第三方库，这个说法是相对于内置库来的，因为内置库毕竟有限，所以需要有第三方库来支持。毕竟代码的格式千千万万，内置库也不可能全部搞定，需要第三方来援助。但是第三方库与内置库在功能上是一致的。如果有一天，第三方服务被银行收编了，呵呵，那么这个第三方库，也就成了内置库了。


### 七、如何学习编程

本来第7个话题是学习JS的方向，但是我把它改成如何学习编程了，因为我确实还没有找到学习JS的方向，不过我可以说说我的大致规划。
因为，我是完全不懂编程，甚至对于操作计算机来说，也不是很熟练。 


学习语言编程，我觉得首先自己要固定好时间，是上午学?还是下午学?每天学多久? 因为我工作性质的原因，我给自己订的目标是每天不低于一个小时，周末不低于三个小时，且每天都要进行，就按着老师的授课顺序来。

根据我这几天的思考，我觉得我只能按着我自己的基础来制定学习进度。没有办法去同他人的进度保持一致，大家的水平相差太多。学编程这个东西，我感觉不比吃饭，嚼烂嚼不烂只管往下吞吞，编程一旦有一个环节没学会，后面的根本进行不下去。

鉴于我的基础，以及我毅力差的性格，我暂时不给自己订学习目标，不打算这个月，或者这个季度，达到某种水平。每天保证学习一个小时以上，哪怕连续几天都在演练同一个项目，那也没关系。

至于具体学习步骤，就是两个字：“试错”，不停的试错。该试的动作，一个都不能拉下，我始终觉得，学习不能走捷径。

有一句话叫做“每天进步一点点，坚持带来大改变。” 能碰到这么具有爱心的“幼儿园老师”，如果不珍惜，恐怕是这一辈子的遗憾。最好的学习方法是什么呢？答案就是“做”。
做，你就对了。


### 班级：JS编程幼儿园

### 学生：王云飞

### 日期：2017.08.12夜


