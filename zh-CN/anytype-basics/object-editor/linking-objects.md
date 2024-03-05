---
Description: How to link your Objects with Relations or Simple Links.
---

# 链接

### 创建新链接

#### 链接到 Anytype 中的另一个对象

直接在画布（canvas）中这样做：

1. **【块链接】。** 输入斜杠字符 ("/") 来唤出命令栏，然后在菜单中寻找 `添加链接到对象（Link to Object）`。这种链接可能以文本或者卡片的形式呈现。
2. **【行内链接】**。输入 @ 即可唤出【对象】选择器菜单。

在弹出的【对象】菜单中选择一个【要关联的某类型对象】，就可以形成【关联】。

#### 链接到设备上的外部对象

如果要在桌面端上添加指向外部【对象】的链接，请以 **file:/// 开头** 然后加上本地文件的目标地址。例如：

* file:///Users/Alex/Downloads/Protocol-Berg.pdf — 打开PDF；
* file:///Users/Alex/Downloads/my\_budget.xlsx — 打开电子表格 (Excel, Numbers)。

要添加这样的链接，与添加新的网页链接一样，选择“链接到网站”（Link to website）。

#### 提及日期

你可以使用 **【行内链接】** 来快速链接到绝对日期或相对日期。

一些例子：

* @now or @today
* @tomorrow
* @nextweek
* @nextmonth
* @24/8/2023

{% hint style="info" %}
遗憾的是，在我们的移动端应用程序上暂未可用。
{% endhint %}

### 检查现有链接

#### 图谱上的关联

在你的文档中，可能会有多个引用或连接，它们连接到你的库中的其他东西。【关联图谱 (Graph)】是可以实现这一点的可视化工具。将【对象】连接到其他【对象】，连接到人（Humans）抑或是任务（Tasks）。

在此处了解有关 [【关联】](../../basics/relations/ "mention") 以及 [【图谱】](../../basics/graph.md "mention") 的更多信息。

![](<../../../.gitbook/assets/image (22).png>)

#### 使用【流程】

检查哪些【对象】被链接在一起的另一种选择是，使用在【图谱 (Graph)】视图中，旁边的【流程 (Flow)】选项卡。

在屏幕顶部中间位置，你能看到切换到 **【流程】** 视图的选项卡。它会显示你当前查看【对象】的前后链接的【对象】。

#### 集锦（Collections）

集锦视图也是使用链接来管理要显示的内容。若要将一个现有的【对象】添加到一个【集锦】中，使用【对象】的上下文菜单（右上角的三点）中的 **添加链接到对象（Link To）**选项。
