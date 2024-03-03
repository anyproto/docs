# 关联（Relations）

### 理解关联 <a href="#understanding-relations" id="understanding-relations"></a>

关联（Relations）是 Anytype 中组织与连接你的【对象】和知识的关键。在 Anytype 中，【关联】有两种功能：

* **定义属性：**你可以使用【关联】来定义某个【对象】的属性。
   * 例如，在 Anytype 中创建一个任务（Task）时，可以添加像 _状态（Status）_ 这样的关联：已完成/未完成，或者 _优先级_：低、中、高。
   * 如果想象成一个数据库，那么【关联】代表的是每一行的列标题（其中 A 列是它的【对象】）。
   * 设置完属性之后，就可以根据在【对象集合】视图中定义的【关联】来对你的【对象】进行排序和筛选。

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMBWIxXziUmcK7h7uvLnI%2Fuploads%2F79DbEaExZn85mNW3Ifsz%2Fimage.png?alt=media\&token=4813e44e-2291-4fe5-9832-6dac24823967)

* **定义联系：**你还可以使用【关联】来将一个【对象】连接到另一个【对象】。
   * 还是以任务为例子，你可以添加这个【关联】：_分配给..（Assignee）_，然后将 Anytype 中的另一个【对象】指定到这个任务。
   * 如上所述，你可以在【对象集合】或【关联图谱】的视图中查看分配给..（Assignee）这个【关联】。
