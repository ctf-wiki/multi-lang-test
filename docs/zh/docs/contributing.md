# 贡献指南

## 写在开头

维护 CTF Wiki 对于个人能力没有太多要求，关键是喜欢开源，愿意花时间做，把自己的所学与他人分享。

在维护 CTF Wiki 的过程中，没有任何指派性的任务，想写什么就写什么，觉得 Wiki 哪里写的不好就完善哪里。

如果觉得之前的人写得不好，可以与其讨论，将其打造为更为合理的结构。

**请务必在看完本部分所有内容后再开始贡献。**


## 交流方式

本项目主要使用 Issue，Discussion 以及 Slack 进行交流沟通。Slack 的团队名为 [CTF-Wiki](https://ctf-wiki.slack.com/join/shared_invite/enQtNTkwNDg5NDUzNzAzLTQ3YTliNzI5OGNhM2NmNzI3NTU0YWRlNWFkY2EzYTExN2Y3ZjRkNzYzYmRhNDNlYmY5YTVmNjNhYjliZDgyNTY)，欢迎加入。

## 贡献方式

### 我之前没怎么用过 Github

参与 Wiki 的编写 **需要** 一个 Github 账号， **不需要** 高超的 Github 技巧。

举个栗子，假如我想要修改一个页面内容，应该怎么操作呢？

1. 在 [CTF Wiki](https://ctf-wiki.github.io/ctf-wiki/) 上找到对应页面
2. 点击 正文右上方、目录左侧的 **“编辑此页”** 按钮
3. （应该已经跳转到了 Github 上的对应页面吧？）这时候右上方还会有一个 **“编辑此页”** 的按钮，点击它就可以在线编辑了
4. 写好了之后点下方的绿色按钮，可能会提示没有权限。不必担心！Github 会自动帮你 fork 一份项目的文件并创建 Pull Request

（有木有很简单？）

如果还是不放心，可以参考这篇文章：https://juejin.im/entry/56e638591ea49300550885cc

### 我之前用过 Github

基本协作方式如下

1. Fork 主仓库到自己的仓库中。
2. 当想要贡献某部分内容时，请务必仔细查看 **[Issue](https://github.com/ctf-wiki/ctf-wiki/issues)** 与 **[Project](https://github.com/ctf-wiki/ctf-wiki/projects)**，以便确定是否有人已经开始了这项工作。当然，我们更希望你可以加入 Slack 中的 [CTF-Wiki](https://join.slack.com/t/ctf-wiki/shared_invite/enQtNTkwNDg5NDUzNzAzLWExOTRhZTE0ZTMzYjVlNDk5OGI3ZDA1NmQyZjE4NWRlMGU3NjEwM2Y2ZTliMTg4Njg1MjliNWRhNTk2ZmY0NmI) 团队，以便于沟通与交流。
3. 在决定将内容推送到本仓库时，**请你首先拉取本仓库代码进行合并，自行处理好冲突，同时确保在本地可以正常生成文档**，然后再 PR 到主仓库的 master 分支上。其中，PR 需要包含以下基本信息
   * 标题：本次 PR 的目的（做了什么工作，修复了什么问题）
   * 内容：如果必要的话，请给出对修复问题的叙述
   * **注意，所有的内容都应该使用英语。**
4. 如果发现 PR 中有什么问题，请在 PR 中直接评论，并尽量给出修正的方式，或者也可以直接进行修改。 
5. 提出该 PR 的人根据评论修正内容，然后将修改后的内容 Merge 到 master 分支中。

目前，在人员较少的前提下，基本上可以忽略 4-5 步。

### 注意
- 每次 Pull Request 应只解决一个主要的事情，这样方便于进行修改。
- 在每次 Pull Request 时，请确保自己在本地生成时，可以正确显示，并在 Pull Request 结束后在对应页面的`Show all checks` 里查看部署是否为自己的期望的样子。
- 如果你想要开启一个新的章节，即编写目前 CTF Wiki 中没有的内容，请务必加入 Slack 中交流，并在交流完毕后 **将自己想要开启的新的章节以简明扼要的方式发起一个新的 issue **。以便于管理人员把这个放到对应 Project 的 In Process 栏中。
- 在你成为团队成员后，你可以自由地编写 Project 中的内容。
- 更多信息，请参见 [F.A.Q](https://github.com/ctf-wiki/ctf-wiki/wiki/F.A.Q)。

## 贡献文档要求

当你打算贡献某部分的内容时，你应该尽量确保

- 文档内容满足基本格式要求
- 文档的合理性
- 文档存储的格式

具体内容参见下面的介绍。

### 文档内容的基本格式

这里主要是指 [中文排版指南](https://github.com/ctf-wiki/ctf-wiki/wiki/%E4%B8%AD%E6%96%87%E6%8E%92%E7%89%88%E6%8C%87%E5%8D%97) 与 [MkDocs 使用说明](https://github.com/ctf-wiki/ctf-wiki/wiki/Mkdocs-%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E)。额外的基本要求如下

- 之后可能会考虑为段落标题自动生成序号，所以我们不推荐在段落标题处增加序号。
- 由于所涉及的题目我们都 **合理** 地放在了 `ctf-challenge` 仓库，所以我们无需在文档中注明题目的链接。而且，题目可能会随时移动，修复链接是一个非常费时间的事情。

### 文档的合理性

所谓合理性，指所编写的 **内容** 必须具有如下的特性

- 由浅入深，内容的难度应该具有渐进性。
- 逻辑性，对于每类内容的撰写应该尽量包含以下的内容
  - 原理，说明该内容对应的原理。
  - 例子，给出 1 ~ 2 个典型的例子。
  - 题目，在该标题下， **只需要给出题目名字**。

### 文档存储的格式

对于每类要编写的内容，对应的文档应该存储在合适的目录下

- figure，存储文档介绍时所使用的图片。需要注意的是，图片要放在本地文件夹，避免引用外链。我们推荐使用相对路径 `./figure` 来索引图片。
- **文件名请务必都小写，以 `-` 分割， 如 `file-name`**
- 注意：无论是例子还是题目，**相应的附件都应该存储在 ctf-challenge 仓库中的对应目录中**。