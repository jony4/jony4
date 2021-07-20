# FSM 有限状态机

## 定义

Wiki -> [有限状态机](https://www.wikiwand.com/zh-hans/%E6%9C%89%E9%99%90%E7%8A%B6%E6%80%81%E6%9C%BA)

状态存储关于过去的信息，就是说：它反映从系统开始到现在时刻的输入变化。转移指示状态变更，并且用必须满足确使转移发生的条件来描述它。动作是在给定时刻要进行的活动的描述。有多种类型的动作：
  - 进入动作（entry action）：在进入状态时进行
  - 退出动作（exit action）：在退出状态时进行
  - 输入动作：依赖于当前状态和输入条件进行
  - 转移动作：在进行特定转移时进行

接受器和识别器（也叫做序列检测器）产生一个二元输出，说要么“是”要么“否”来回答输入是否被机器接受。所有FSM的状态被称为要么接受要么不接受。在所有输入都被处理了的时候，如果当前状态是接受状态，输入被接受，否则被拒绝。作为规则，输入是符号（字符）；动作不使用。图2中的例子展示了接受单词"nice"的有限状态自动机，在这个FSM中唯一的接受状态是状态7。

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a8/Fsm_parsing_word_nice.svg/800px-Fsm_parsing_word_nice.svg.png)

变换器使用动作基于给定输入和／或状态生成输出。它们用于控制应用。常分为两种类型：米利（Mealy）机和摩尔（Moore）机，米利机的下一状态和输出取决于当前状态和当前输入；摩尔机的下一状态取决于当前状态和当前输入，但其输出仅取决于当前状态。

![image](https://user-images.githubusercontent.com/13718575/118110130-9cec2780-b414-11eb-8f68-82cbf104d69e.png)
![image](https://user-images.githubusercontent.com/13718575/118110167-ab3a4380-b414-11eb-8315-f0f582aa75f9.png)


有限状态自动机在很多不同领域中是重要的，包括电子工程、语言学、计算机科学、哲学、生物学、数学和逻辑学。有限状态机是在自动机理论和计算理论中研究的一类自动机。在计算机科学中，有限状态机被广泛用于建模应用行为、硬件电路系统设计、软件工程，编译器、网络协议、和计算与语言的研究.

## Go Langauge Impl
  - [fsm](https://github.com/looplab/fsm)

## Docs
  - [A Simple State Machine Framework in Go](https://venilnoronha.io/a-simple-state-machine-framework-in-go)

## 应用
下列概念经常用来建造有有限状态机的软件应用：
  - 事件驱动FSM
  - 虚拟FSM (VFSM)
  - 基于自动机编程

  ### 前端应用
  - [David Khourshid: Simplifying Complex UIs with Finite Automata & Statecharts | JSConf Iceland 2018](https://www.youtube.com/watch?v=RqTxtOXcv8Y&ab_channel=JSConf) YouTube
  - [David Khourshid - Infinitely Better UIs with Finite Automata](https://www.youtube.com/watch?v=VU1NKX6Qkxc&ab_channel=ReactRally) YouTube

  ### 后端应用
  - [BPMN](https://www.omg.org/spec/BPMN/2.0.2/)
  - [Wedo](https://github.com/wedo-workflow/wedo)
  - [基于有限状态机的工作流引擎的设计.pdf](http://www.shcas.net/jsjyup/pdf/2018/8/%E5%9F%BA%E4%BA%8E%E6%9C%89%E9%99%90%E7%8A%B6%E6%80%81%E6%9C%BA%E7%9A%84%E5%B7%A5%E4%BD%9C%E6%B5%81%E5%BC%95%E6%93%8E%E7%9A%84%E8%AE%BE%E8%AE%A1.pdf) 
