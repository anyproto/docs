<p align="center">
    <a href="https://doc.anytype.io">
        <img src="../.gitbook/assets/anytype-logo-360px.png" alt="Docs-Logo" width="100px" height="100px">
    </a>
</p>


## 目录

- [**简介**](#Intro)
- [**贡献流程**](#contribution-process)
- [**文件结构**](#file-structure)
- [**约定**](#conventions)
   - [**文本格式**](#text-formats)
   - [**列表**](#lists)
   - [**块（Blocks）**](#blocks)
   - [**媒体**](#media)

## 简介

ℹ️我们要求所有用户在贡献文档之前阅读我们的 [行为守则](https://github.com/anytypeio/community/blob/main/README.md#code-of-conduct) 和 [Gitbook 公约](#conventions)。
欢迎在 PR 中提出任何修改建议，并参与 [改进 doc.anytype.io](https://community.anytype.io/t/improvements-for-doc-anytype-io/2862) 主题的讨论。请按照一下步骤进行贡献。如果你是 \_git\* 和/或 _GitHub_ 的新用户，我们建议你阅读 [GitHub 指南](https://guides.github.com/introduction/flow/)。


## 贡献流程

1. 分叉该版本库（Fork）
2. （可选）克隆分叉（Clone）
   - 使用 SSH
      ```shell
      git clone --filter=tree:0 git@github.com:anytypeio/community.git
      ```
   - 使用 HTTPS
      ```shell
      git clone --filter=tree:0 https://github.com/anytypeio/community.git
      ```
   - 使用 GitHub CLI
      ```shell
      gh repo clone anytypeio/community -- --filter=tree:0
      ```
3. 从 `main` 创建新的分支（branch）
4. 在新分支上进行更改
5. 提交并推送到新分支（Commit & push）
6. 提出拉取请求（pull request，PR）
7. 指定 [Vladimir](https://github.com/d1eselboy)、[Divyanshu](https://github.com/div3xi) 或 [Enda](https://github.com/endac) 为 PR 的审核人。

## 文件结构

* 文档中添加或删除的任何页面都需要添加到 [SUMMARY.md](https://github.com/anytypeio/docs/blob/main/SUMMARY.md) 文件的 **目录** 中。
   * 缩进用于表示页面的嵌套（于子文件夹中）
   * 使用 markdown 的 URL 表示方式来链接页面，例如：
      ```
      [导航](https://github.com/anytypeio/docs/blob/main/features/navigation.md)
      ```
* 所有文件都以 **Markdown（.md）** 格式保存
* 对于子文件夹中的嵌套页面，需要被放在类别文件夹中。如果类别文件夹不存在，则你可以创建该文件夹
* 要使用图片，必须全部放在 [.gitbook/assets](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) 文件夹中，然后从该文件夹中引用图片
   > 所有媒体都应使用浅色模式
## 约定

> 以下是在 Gitbook 上创建 markdown 格式文档时要遵循的规则。请在进行任何修改时遵循这些规则。

### 文本格式

- # 一级标题
   ```
   # 一级标题
   ```

- ## 二级标题
   ```
   ## 二级标题
   ```

- ### 三级标题
   ```
   ### 三级标题
   ```

- **粗体**
   ```
   **粗体文本**
   ```

- *斜体*
   ```
   _斜体文本_
   ```

- ~~删除线~~
   ```
   ~删除线文本~
   ```

- 水平分隔线
   ```
   ---
   ```

- [URL](#)
   ```
   [URL 名称](https://example.com)
   ```

- ![图片](#)
   ```
   ![图片](http://url/a.png)
   ```

- `行内代码`
   ```
   `行内代码`
   ```

### 列表

- **无序列表**
   ```
   * 项目 1
   * 项目 2
   * 项目 3
       或
   - 项目 1
   - 项目 2
   - 项目 3
   ```

- **有序列表**
   ```
   1. 项目 1
   2. 项目 2
   3. 项目 3
   ```

- **任务列表**
   ```
   * [ ] 未勾选任务
   * [x] 已勾选任务
   ```

### 块（Blocks）

- **代码块**
```
```   创建一个新代码块。
```py   使用 Python 语法高亮来创建一个新代码块。
```

- **引用**
   ```
   使用 > 来开始一个引用块。
   ```

- **信息提示块**
   ```
   {% hint style="info" %} 信息提示块 {% endhint %}
   ```
   <p align="left">
       <a href="https://doc.anytype.io">
           <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/info-hints-block.png" alt="info-hints">
       </a>
     </p>

- **警告提示块**
   ```
   {% hint style="warning" %} 警告提示块 {% endhint %}
   ```
   <p align="left">
       <a href="https://doc.anytype.io">
           <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/warning-hints-block.png" alt="warning-hints">
       </a>
     </p>

- **成功提示块**
   ```
   {% hint style="success" %} 成功提示块 {% endhint %}
   ```
   <p align="left">
       <a href="https://doc.anytype.io">
           <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/success-hints-block.png" alt="success-hints">
       </a>
     </p>

- **危险提示块**
   ```
   {% hint style="danger" %} 危险提示块 {% endhint %}
   ```
   <p align="left">
       <a href="https://doc.anytype.io">
           <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/danger-hint-block.png" alt="danger-hints">
       </a>
     </p>

### 媒体

- **块：** 要创建一个媒体块，需要遵循以下约定
   ```
   ![媒体标题](<.gitbook/assets/file-name>)
   
   例：
   
   ![主页](<.gitbook/assets/Screenshot 2021-11-05 at 18.45.31.png>)
   ```
   当你添加媒体块时，如果正在编辑的页面处于子文件夹中，请使用在相对路径中适当次数的上层目录 `../` 以使嵌入生效。

- **文件存储：**任何媒体都必须先上传到 [.gitbook/assets/](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) 文件夹。然后才可以在文档中使用。你可能会在现有的页面中看到 GitBook 独有的嵌入格式 `{% embed url="，但你不需要使用这种格式。

- **文件格式：**这些是在文档中上传媒体时唯一可接受的文件格式。
   - **视频：**

      > ✔ 仅使用 **MP4**
      > ❌ 不要用 **gif** 或其他格式

   - **图片：**

      > ✔ 仅使用 **PNG** 和 **JPG** 图片
      > ❌ 不要使用其他格式

- **大小限制：**每个上传媒体文件的大小限制为 **5 兆字节（MB）**。1000px 宽度的图片和视频仍然可以非常清晰地显示，将 4k 文件大小减少了大约 75%。

- **命名：**为了减少混淆，上传文件时，请以人类可读的格式重新命名你的文件
   ```
   <图片标题>-<页面>.<文件格式>
   
   例：
   ✔️ loadingscreen-intro.png
   ❌ Screenshot 2021-11-05 at 18.45.31.png
