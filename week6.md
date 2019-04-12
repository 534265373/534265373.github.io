### 简答题

**1. 用例的概念**   
在软件和系统工程中，用例是通常定义角色（在统一建模语言（UML）中称为参与者）和实现目标的系统之间的交互的动作或事件步骤的列表。演员可以是人或其他外部系统。在系统工程中，用例的使用范围高于软件工程中的用例，通常代表任务或利益相关者目标。然后可以在系统建模语言（SysML）中或作为合同语句捕获详细要求。  

**2. 用例和场景的关系？什么是主场景或 happy path？**  
场景是actors和系统之间特定的一系列动作和绘画，是用例的实例。一个用例是一些场景的集合。  
主场景（基本流）对应系统的主要的交互，通常是“成功”的场景。主场景是最常用的，能直接地实现用户目标的流程。  

**3. 用例有哪些形式？**  
Brief： 简短的一段总结，通常是主要的成功场景；在早期需求分析过程中，快速了解主题和范围；可能只需用几分钟来创建。    
Casual： 非正式的段落格式；覆盖多个场景的几个段落；在早期需求分析过程中，快速了解主题和范围。  
Fully： 所有的步骤和变化都写得很详细，以及先决条件和成功保障等支撑部分；所有的用户样例都已经确定且简略写完后，在第一个需求研讨会期间，一些（例如10%）架构上重要的和高价值的用例需要被详细地编写。  


**4. 对于复杂业务，为什么编制完整用例非常难？**  
复杂业务的子用例非常多，流程复杂，且需要处理的场景很多。因此很难考虑完全所有子用例和场景，且绘制的用例图繁杂，容易出错。  

**5. 什么是用例图？**  
用例图是指由参与者、用例，边界以及它们之间的关系构成的用于描述系统功能的视图。用例图是外部用户（被称为参与者）所能观察到的系统功能的模型图。用例图是系统的蓝图。用例图呈现了一些参与者，一些用例，以及它们之间的关系，主要用于对系统、子系统或类的功能行为进行建模。  

**6. 用例图的基本符号与元素？**  
系统（System）：图中的大方框，可以是小型软件组件，也可以是完整的应用程序，里面包含外部可见的功能。
  
参与者（Actor）： 表示的是一个系统用户，也就是与应用程序进行交互的用户、组织或外部系统。  
![1](/images/hw6/actor.png)  
  
用例（Use Case）： 表示的是对系统提供的功能、服务的一种描述。  
![2](/images/hw6/use_case.png)  
  
包含关系（Include）： 表示用例可以简单地包含其他用例所具有的行为，并把它所包含的用例行为作为自身行为的一部分。  
![3](/images/hw6/include.png)  
  
扩展/延伸关系（Extend）： 表示在一定条件下，把新的行为加入到已有的用例中，获得的新用例叫做扩展用例，原有的用例叫做基础用例，相当于为基础用例提供一个附加功能。  
![6](/images/hw6/extend.png)  
  
泛化关系（Generalization）： 泛化指的是一个父用例可以被特定化形成多个子用例，而父用例和子用例之间的关系就是泛化关系。  
![4](/images/hw6/generalization.png)  
  
关联关系（Association）： 表示的是参与者与用例之间的关系。  
![5](/images/hw6/association.png)  
  
**7. 用例图的画法与步骤**
需求识别：确定研究对象，需要研究一个什么样的系统，系统名写在上方正中间。  
识别参与者：确定系统中的参与者，包括主要参与者，协作参与者，幕后参与者。  
识别用例：确定需要研究的系统中的用例和服务，区分用户级别的用例和子用例。   
建立用例与参与者（Actor）之间的关系：确认用例间的关系，确认用例与参与者之间的关系。   

**8. 用例图给利益相关人与开发者的价值有哪些？**
对利益关系人：明确系统的业务范围、服务对象（角色）、外部系统与设备。可以直观看到系统的功能和操作过程，保证系统按用户的需求进行设计。
对开发者：帮助识别技术风险，提前实施关键技术原型攻关。使得开发者能够更明确地获得需求，更好地理解需求。可以指导开发和测试，同时可以在整个过程中对其他工作流起到指导作用。


### 建模练习题（用例模型）

- 选择2-3个你熟悉的类似业务的在线服务系统（或移动 APP），如定旅馆（携程、去哪儿等）、定电影票、背单词APP等，分别绘制它们用例图。并满足以下要求：
  - 请使用用户的视角，描述用户目标或系统提供的服务
  - 粒度达到子用例级别，并用 include 和 exclude 关联它们
  - 请用色彩标注出你认为创新（区别于竞争对手的）用例或子用例
  - 尽可能识别外部系统和服务
  
  淘票票  
  ![6](/images/hw6/uml1.png)  
  
  背单词 
  ![7](/images/hw6/uml2.png) 