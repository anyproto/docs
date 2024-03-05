---
description: Contributed by our user Roland
---

# 基本概念介绍

前言

因为我自己的认识并不是从官方的资料中来，而是自己在使用过程中摸索出来的，所以可能与官方描述存在偏差，仅作为参考。

我将分层级介绍Anytype中几个重要功能的概念。

关于这些概念，有必要先打一个预防针，Anytype在笔记形式的理念上是相较于大多数笔记软件是要更加前卫，下文提到的概念的名字，即使是在英语中也不能够只从字面上去理解，这些功能的真正的名字或许还没有在这个时代诞生，现在所用的名字只是借用了一些可能会在某方面相似的概念的名字，如果从这些名字来看，我们对于它们所习惯的用法可能会让我们的认知产生误解，所以最好将这些名字作为代号来看待，名字和定义都不去管吧，最好从这些功能能够怎么去用的角度去感受它们的实质。

本篇内容，只需要看看，在本篇的介绍完成之后，会另有下文去介绍我如何去使用Anytype，在后文的用例中更能体现一些深入的理解，这会比琢磨定义和意思更直接。

另外，我的用法不一定适合大家，但是相信大家可以从我的用法中找到可以借鉴的点，希望我的分享可以让更多人少走我所走的弯路。

#### Object、Type、Relation

**Object**

在Anytype中，我们的每一条笔记及类似的东西，被称为Object。

**Type**

不同类型的笔记、对象应该被用不同的方式管理，这是我们划分type的好处。

不同的type可以分别设置不同的模版和其他参数。

**Relation**

Relation是从Notion的Database演化而来的，区别在于：Relation能够更加灵活地与Object产生联系。

Relation的主要用途是从各个角度描述Object，就像是一个Object的各方面参数一样，以便于后续筛选、排序与关系整理。

Relation的细分类如图所示。

<figure><img src="https://lh4.googleusercontent.com/VHcTvl7yMA-SvEMyGRTp3mykoWESuoHgROXwcyLGnFuwdg0vcoYRFZ5nJjM6ctvfL7EcgHEogn6JFbrbKKH90ow4mjgrwQTXEPnzMcNEHfeB4joxImzoGiOZ34goRwtG322E_VZZ4c536KYjpcAGvieql3bXrQag" alt=""><figcaption></figcaption></figure>

#### Set、Collection

在Anytype中，我们无法直接在type的界面对属于这个type的object进行修改，需要在set和collection中进行操作。

**Set**

set，意为数学概念中的“集合”，我们可以从type的页面处创建

<figure><img src="https://lh4.googleusercontent.com/xWHkmtuuXvM7WZKUScZBJ6kqD0cYhKfhVxBVLXFrIKWIAwgp1ATOTdsTwWl6QZ2RmUWhO728jygX5HqcWsadgy3OL6jIwwqHjJnFVFYIDhgqSxdCpXC1hnAegQpi_xj_xpbnoNlsAxLzDJPGbZvsfv7kFGhpng53" alt=""><figcaption></figcaption></figure>

然后，这个type的所有object将会显示在set页面中，对于每一个type，我们都能够进行这个操作来创造出对应的set来管理，不过建议用到的时候再说。

一个set下可以有多个视图，如图红框所示。在每一个视图下可以进行筛选、排序、选择视图类型（网格、画廊、列表、看板）。在最新的beta版本中，每个视图可以选择这个视图下创建object时的默认模版。

<figure><img src="https://lh5.googleusercontent.com/kTUmzJ0JN4lAQNxa_tEh-TNy1YOwsqmg3X3OOLKVZzjiDbQrHM1uAj1SrEePLsIyAI4wKXxDBqBShQKj7uurP2rf87dwfwQIxPSKtaY5ZYxZdzE1_zLOUOYCrwwiUS0bQjBSFzRuSsilsJ3AUbSvQKRhAN1T5akS" alt=""><figcaption></figcaption></figure>

关于set的使用方法建议，会在下方用例分享的部分中展开说明。

**Collection**

Collection是一种特殊的set，set里面只会有对应type的object，而Collection里面可以含有多种type。

我们可以在collection里面创建Object；

也可以将已有的Object连接到Collection，如此一来这个Object也会显示在Collection里面。

#### Tag（Relation）

这些概念基本介绍完了，这里再单独介绍一下Tag这个Relation类型，它将会是后面用例文章中实现无层级无文件夹结构化的关键抓手。

我们可以创建一个tag类型的Relation，名字可以自己设置，这里以“测试Tag”为例。

可以输入来选择已有的Tag或者创建一个新Tag

<figure><img src="https://lh3.googleusercontent.com/1-k_qukc__r7FGx2QNUghqHQ0FReyjRG9-qHavNthpGvFdAreXHOoZO27n1-ZSGqbyxpIRfek-w5uGpxns4nRYUMqI5CZYMgdYIcY_jJ6L4NUAQtA6AfNmkmFG-b8rL2oPKkW50beGsK3S57oEzkeCFBiUT_eE7w" alt=""><figcaption></figcaption></figure>

当然不仅可以有一个tag的relation，这里就有很大的发挥空间了。

<figure><img src="https://lh5.googleusercontent.com/MvhP2tfMhLhMbLRACY-zhYW42n7XwSgFkGMTltl1EiNbO4qrnotxuE1z-T6Jh_jLkXf0Q8kDdNaeKSBBwPcW6I0eF5oJ38_WkD0gk0pBVVZUkxO4dKMypyKGlKkiNiw6_4SzExhICiKVyuSKAFYgfh3PdKR8-eLU" alt=""><figcaption></figcaption></figure>

大概的功能介绍这里就结束了，总结来说，对于Anytype中的概念，与其去纠结名字和定义，关注它们能够用来做什么，能够比较有效地认识。

#### 个人用例分享——Set的使用模式建议

**前言**

这一部分将介绍个人使用Anytype过程中建立起来的一个模式，看之前建议先看《Anytype入门1——基础功能的了解》。

因为每个人的需求和使用目标可能有无法预料的差异，因此用法仅作参考，不过我相信我的用法多少能给大家带来一些启发。

**这种方法的特点**

契合原子化的结构，不需要文件夹结构和层级结构

利用标签进行结构化，支持灵活分类，支持交叉分类

**使用更少的Type进行管理**

虽然按不同的Type进行管理会有其好处，但是过度地划分Type也会存在隐患。

在Anytype中，Object必然属于某一Type（不存在不属于任何Type的Object），并且Object的Type只能有一个（不存在同时属于多个Type的Object）。

因此，如果Type分的太多，很容易产生“这个Object要属于哪个Type”的问题。

因此我从一开始的细分type（如日记、日语词汇、英语词汇、想法记录、词条等等）的模式转向大type模式（除特殊类型的Object外，一律使用Page这个type管理），将分类这个事情从多个type之间转移到type内部。

**使用Tag进行Type内部的灵活分类**

在基本概念介绍的部分中，已经提到过，Tag可以用来灵活分类。

在我的Page这个type中，几乎包含了我大多数的的Object，我主要使用Tag来管理它们。

<figure><img src="https://lh6.googleusercontent.com/9YNXjyNywK02V7JNUK95BWqRhiQ_o7s37WXkQw2QURrLAwpTckzMMhtBd3ca3w6JW7WvXDUdFRQTv07zGs_Ecwz-8xgbNa0b-r6B2gb5qW--G5dKDCWYSWtvURVWvTZqiDwPhnyV4X4dhFWPGvq2JWXnXcPGOoUI" alt="" width="375"><figcaption></figcaption></figure>

为了方便自己着重地浏览某个小类的Page，比如所有的摘录，我会在Set的选项卡这里新建一个选项卡，在Page的基础上筛选出所有Page类型这个Relation中包含摘录这个标签的页面。

<figure><img src="https://lh6.googleusercontent.com/s91Pgl7dEshMLbZL6ZtDTZdJJDMdW1YbDMGWICqupNIZtJJ9yRkcJjz-A8T85WKCG0gBFfVwxVQt595DA5JEP7OQ8Ju3vcHAMY_9Jjhdp2vVuof5Is-wOncFPn4kVQZB_nCHsAGJngVDQPbBCvh0iuIsa32W17H_" alt=""><figcaption></figcaption></figure>

筛选出来效果如下图

<figure><img src="https://lh6.googleusercontent.com/rQBnOGAr9gBZYX0SkHzftWCJAzrtzEsBEcF7o7V8Q7QX2qQOK_aJZ8FLFVFgCUEnBEAU24N4HkMF4lawniRyevk3i7Aw6VLVh54KWY1PM9uVP4eZfDRkDsBSYXICrpO9TzOne2A-HRmC6-PFudBypQYeq1PMjmn8" alt=""><figcaption></figcaption></figure>

为了方便大家理解我将Page类型在这个页面也展示出来了。

我们还可以根据这个小类的特点进行特别的管理，比如摘录这个类型的Page大多数都使用了“作者”这个Relation，我们在这个标签页中可以单独地显示出来。

这个筛选结果和设置显示出来的Relation，是保留并且维持下去的，不需要每一次打开都重新设置，我们可以修改标签页的名字为“摘录”来提醒自己这是这个页面显示的全是摘录。

\
**各个视图下设置默认模版**

在最近的0.34.0版本更新后，我们为每个视图设置单独的默认模版，这样一来我这种用法会更加的顺畅，可以根据为Page Type下面的每个小类单独设置默认模版。

<figure><img src="https://lh3.googleusercontent.com/L55edepq-7yuybCBCZXX43cbVcltyHYWfvTEtLYhZZLtXYGv4FirwrJ-Qn_i8lpWD8tBriTKse6bzZYPCzo30au8_0dHKx2PaSeUO2V0FU4xQ1kEFeAwHLzpFCOuoGojja2v_tgOacbrc5rus6di7YnSniAkSj6U" alt=""><figcaption></figcaption></figure>

**Tag的使用心得**

在Anytype中，同一个Tag的Relation，包含的所有标签是互通的（已经存在的标签会成为后续添加标签的可选项），我为了更好的管理这些标签，在每个type下面创造了对应分类用的Tag Reletion，如Page Type下我会用“Page类型”这个Tag Relation进行管理，而Human type则用“Human类型”进行管理，这样子它们之间的选项不会串。

Tag的灵活分类，使得我们在设立分类的时候不需要考虑两种类型是否互斥，例如我用来管理Page的类型有主题笔记、词条、手稿、灵感记录、想法记录、清单记录、日记、中文词汇、日文词汇。

可以看到，这些分类中有一些很暧昧，一些的划分角度跟另外一些看起来有明显的区别，这就是Tag分类的灵活性——我们不需要预先对分类进行严格的划分、不需要保证他们是互斥的、不需要强制自己按特定的角度进行划分。

而对于Object来说，我们既可以是它不属于任何一个分类，也可以同时属于多个分类，很灵活。

个人对于Tag在这方面发挥的作用，比起分类更像是“助记词”，因此打标签的时候，我会更加的随心，按照自己的想法来。等到我需要找到这个页面的时候，我就可以很自然地想起这个页面是什么标签，因而快速地筛选出来。这种助记词一样的tag使用方法，在原子化的笔记结构中是很好用的，当软件中的object多起来的时候，会体现的更加明显。

**该用法的额外好处——原子化结构的进一步体现**

使用上述的方法可以对内容进行灵活分类且允许交叉分类，回到跟Notion等软件的Database Like功能中去对比的话，我们发现，其他软件中的Database的结构和用法受到了其表格形式的限制，可以视为一个加强版的表格，但是其下内容的组织也受到了表格使用习惯的影响——我们必须决定这个表格的主题后才能进行其中内容的写入，也就是说，我们在写入的时候必须先考虑好我们之后要以什么样的主题、视角去使用。

而我在上面所推荐的用法，则切断了这种绑定，我们可以像用其他软件一样地去组织内容（即我原先使用的大Type模式，或者使用Collection按特定的角度或者主题去组织起来），但也有了这以外的选择。这意味着我们在创建和编辑Object的时候不再需要考虑实际使用的时候要采用什么角度，这导向了一种更加无摩擦、无感的笔记使用方式——内容的创造和使用脱离了彼此的束缚，自由地创造以及自由地从各个角度组织、使用起来。
