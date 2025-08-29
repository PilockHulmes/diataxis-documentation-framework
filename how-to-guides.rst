.. _how-to:

操作指南
=============

..  rubric:: 操作指南是通过 **步骤指引** 带领读者解决问题或实现结果的指导性文档，其本质是 **以目标为导向** 的实用说明。

===========

操作指南帮助用户正确且安全地完成某项任务；它引导用户的 *行为*。

它关注的是*实际工作*——如何在实际问题领域中实现从一端到另一端的导航。

..  image:: /images/overview-how-to.png
    :alt: How-to guides - task oriented, practical steps, that serve our work
    :class: sidebar

例如： *如何校准雷达阵列*； *如何在 pytest 中使用 fixture*； *如何配置重连退避策略*。另一方面， *如何构建 Web 应用程序* 则不属于此类——这并未针对特定目标或问题，而是一个极度开放式的技能领域。

操作指南的重要性不仅在于用户需要完成任务：文档中的操作指南清单有助于勾勒出产品实际 *功能* 的图景。丰富的操作指南列表能有效暗示产品的能力范围。

针对正确问题撰写的优质操作指南，往往会成为文档中被阅读最频繁的部分。

=================

操作指南针对具体问题
-----------------------------------

**操作指南必须从用户视角而非机器视角编写**。操作指南代表用户需要完成的具体任务，换言之，其内容应由用户需求定义。每篇操作指南都应服务于用户的实际项目，明确展示用户如何利用现有工具达成目标结果。

这与当前普遍存在的操作指南模式形成鲜明对比——后者通常将操作指南定义为针对某个工具或系统可执行的操作步骤。这种模式的弊端在于它几乎无法为用户创造实际价值。这些指南并未针对用户的任何实际需求。相反，它们聚焦于工具本身，机械性地演示操作流程。

这本质上是一种 *意义性* 的区分。意义由目的和需求赋予。机器的功能运作中不存在目的或需求，它仅仅是因果链条的输入与输出。

考虑以下示例：

* "为了关闭水流，请顺时针旋转水龙头。"
* "要部署所需的数据库配置，请选择相应选项并点击 **部署**。"

..  sidebar:: 
    
    我们确实不需要被告知如何用电源开关启动设备，但令人震惊的是，软件文档中的操作指南却常常停留在这个水平。

上文的示例 *看似* 属于操作指南，实则并非如此。

这些内容大多属于无用信息——任何具备基础能力的人（即在该领域工作的人员）都应掌握这些常识。标准化接口与普遍预期知识相结合，应当能清晰呈现大多数操作的实际效果。

其次，它们与使用目的脱节。用户真正需要了解的信息可能包括：

* 针对特定用途，应调节多大的水流强度及水量
* 哪些数据库配置选项符合实际业务需求

..  sidebar:: 
    
    操作指南应聚焦目标、项目与问题，而非工具本身。
    
工具在操作指南中往往作为辅助角色出现，是实现用户目标的途径。当然，当特定目标与特定工具或系统组件紧密关联时，您会发现该操作指南确实会重点讨论该工具。同样常见的是，操作指南会横跨系统中的不同工具或组件，通过一系列由用户需求定义的操作将它们串联起来。无论是哪种情况，操作指南的覆盖范围都由具体项目需求决定。


=================

操作指南的边界定义
--------------------------

**操作指南与教程截然不同**。 尽管常被混淆，但二者服务的用户需求存在本质差异。将两者混为一谈正是导致文档问题的根源所在。关于这一区别的详细讨论，请参阅 :ref:`tutorials-how-to` 这一节。

另一个常见的误解是将操作指南简单等同于流程说明。但解决问题或完成任务并非总能简化为线性流程，现实问题往往不适用于按部就班的解决方案。操作指南中的动作序列有时需要分叉和重叠，并且具有多个入口点和出口点。通常，操作指南需要用户依靠自身判断来应用其提供的指导。
    

=================

核心原则
---------------------------------------

操作指南聚焦于具体工作——以解决任务或问题为导向， *始终围绕实践目标展开*。

..  sidebar:: 操作指南特性

    * 聚焦任务或问题
    * 假设用户明确目标
    * 仅呈现操作步骤
    * 杜绝偏离、概念解析或教学

任何额外添加的内容都会分散您和用户的注意力，削弱指南的实用价值。常见的诱惑是进行概念解析或为了完整性提供参考内容。这些都不属于引导用户完成工作的范畴。它们会阻碍实际操作；如果确实重要，请以链接形式提供。

操作指南服务于已具备能力的用户，这类用户明确知晓自身需求，并能准确遵循您的指引执行操作。


应对现实复杂性
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**A how-to guide needs to be adaptable to real-world use-cases**. One that is useless for any purpose except *exactly* the narrow one you have addressed is rarely valuable. You can't address every possible case, so you must find ways to remain open to the range of possibilities, in such a way that the user can adapt your guidance to their needs.

Omit the unnecessary
~~~~~~~~~~~~~~~~~~~~

In how-to guides, **practical usability is more helpful than completeness.** Whereas a tutorial needs to be a complete,
end-to-end guide, a how-to guide does not. It should start and end in some reasonable, meaningful place, and require
the reader to join it up to their own work.


Provide a set of instructions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A how-to guide describes an *executable solution* to a real-world problem or task. It's in the form of a contract: if you're facing this situation, then you can work your way through it by taking the steps outlined in this approach. The steps are in the form of *actions*.

"Actions" in this context includes physical acts, but also thinking and judgement - solving a problem involves thinking it through. A how-to guide should address how the user thinks as well as what the user does.


Describe a logical sequence
~~~~~~~~~~~~~~~~~~~~~~~~~~~

The fundamental structure of a how-to guide is a *sequence*. It implies logical ordering in time, that there is a sense and meaning to this particular order.

In many cases, the ordering is simply imposed by the way things must be (step two requires completion of step one, for example). In this case it's obvious what order your directions should take.

Sometimes the need is more subtle - it might be possible to *perform* two operations in either order, but if for example one operation helps set up the user's working environment or even their thinking in a way that benefits the other, that's a good reason for putting it first.


Seek flow
~~~~~~~~~

At all times, try to ground your sequences in the patterns of the *user's* activities and thinking, in such a way that the guide acquires *flow*: smooth progress.  

Achieving flow means successfully understanding the user. Paying attention to sense and meaning in ordering requires paying attention to the way human beings think and act, and the needs of someone following directions. 

Again, this can be somewhat obvious: a workflow that has the user repeatedly switching between contexts and tools is clearly clumsy and inefficient. But you should look more deeply than this. What are you asking the user to think about, and how will their thinking flow from subject to subject during their work? How long do you require the user to hold thoughts open before they can be resolved in action? If you require the user to jump back to earlier concerns, is this necessary or avoidable?

A how-to guide is concerned not just with logical ordering in time, but action taking place in time. Action, and a guide to it, has pace and rhythm. Badly-judged pace or disrupted rhythm are both damaging to flow.

At its best, how-to documentation gives the user flow. There is a distinct experience of encountering a guide that appears to *anticipate* the user - the documentation equivalent of a helper who has the tool you were about to reach for, ready to place it in your hand. 


Pay attention to naming
~~~~~~~~~~~~~~~~~~~~~~~~

**Choose titles that say exactly what a how-to guide shows.**

* good: *How to integrate application performance monitoring*
* bad: *Integrating application performance monitoring* (maybe the document is about how to decide whether you should, not about how to do it)
* very bad: *Application performance monitoring* (maybe it's about *how* - but maybe it's about *whether*, or even just an explanation of *what* it is)

Note that search engines appreciate good titles just as much as humans do.

==============

The language of how-to guides
-----------------------------

*This guide shows you how to...*
    Describe clearly the problem or task that the guide shows the user how to solve.
*If you want x, do y. To achieve w, do z.*
    Use conditional imperatives.
*Refer to the x reference guide for a full list of options.*
    Don't pollute your practical how-to guide with every possible thing the user might do related to x.


================

Applied to food and cooking
---------------------------

Consider a recipe, an excellent model for a how-to guide. A recipe clearly defines what will be achieved by following it, and **addresses a specific question** (*How do I make...?* or *What can I make with...?*).

..  image:: /images/old-recipe.jpg
    :alt: A recipe contains a list of ingredients and a list of steps.

It's not the responsibility of a recipe to *teach* you how to make something. A professional chef who has made exactly the same thing multiple times before may still follow a recipe - even if they *created* the recipe themselves - to ensure that they do it correctly.

Even following a recipe **requires at least basic competence**. Someone who has never cooked before should not be expected to follow a recipe with success, so a recipe is not a substitute for a cooking lesson.

Someone who expected to be provided with a recipe, and is given instead a cooking lesson, will be disappointed and annoyed. Similarly, while it's interesting to read about the context or history of a particular dish, the one time you don't want to be faced with that is while you are in the middle of trying to make it. A good recipe follows a well-established format, that excludes both teaching and discussion, and focuses only on **how** to make the dish concerned.
