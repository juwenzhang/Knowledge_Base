## 仓库介绍

* 该仓库使用来实现的是将所有的学习的部分按照不同的分支进行存储的一个仓库

### Typora MarkDown 基础语法

* #### 为什么写这个耶？？

  ```
  因为我们书写 readme.md 的时候，或者说书写 GitHub 的个人主页的时候，我们都是需要使用我们的这个 markdown 的语法进行美化
  
  自己的对应的项目的介绍的，所以说就不得不提一些 关于 markdown 编辑的时候的一些好用的语法格式了
  ```

* #### MarkDown 的应用场景

  ```
  可以用来书写我们的 GitHub 项目的解释文档以及可以支持我们的在线阅读
  ```

* #### 标题的书写

  ```
  # 一级标题  ctrl + 1
  ## 二级标题  ctrl + 2
  ### 三级标题  ctrl + 3
  
  最多支持六级标题
  ```

* #### 分割线的书写

  使用三个以上的 `*` `-` 或者 `_` 表示的就是分割线

  ```
  ***  就是分割线的书写
  
  ---  也是分割线的书写
  
  ___ 也是分割线的书写
  ```

  ***

  ___

  ---

  

* #### 文本格式

  ``` 
  *文本*  就是表示的是文本是我们的斜体
  
  **文本**  就是表示的是我们的文本加粗
  
  ~~文本~~  就是表示的是删除线
  ```

  *hello world*

  **hello eorld**

  ~~hello world~~

* #### 表情符号

  ```
  :smile:
  :heart:
  ```

  :smile:  :heart:

* #### 列表

  ```
  - 
  * 
  +
  上面的三个符号都是表示的是无序列表
  ```

* #### 引用

  ```
  > 第一个引用
  >> 嵌套引用
  ```

  >

  > >

* #### 行内代码

  ```
  `代码内容`
  ```

  `hello world`

* #### 代码块

  ```
  ​```
  	代码块内容
  ​```
  
  ​```java
  	java 代码
  ​```
  ```

* #### 上标和下标

  ```
  <sub>下标</sub>
  
  <sup>上标</sup>
  ```

  **hello world <sub>1</sub>**

  **hello world <sup>2</sup>**

* #### 图片和链接引入

  ```
  链接引入:
  [名称](url)  ctrl + k
  
  
  图片引入
  ![名称](url)
  ```

  ![]()

  []()

* #### 注释

  ```
  <!-- 注释内容 -->
  ```

  <!--hello eorld-->

* #### 表格

  ```
  ctrl t
  ```

  |      |      |      |
  | :--: | ---- | :--: |
  |      |      |      |
  |      |      |      |
  |      |      |      |

## Github 操作

* ### 拉取项目

  ```
  通过 https 进行拉取项目
  git clone https://github.com/juwenzhang/Knowledge_Base.git  
  
  通过 SSH 进行拉取项目
  git clone git@github.com:juwenzhang/Knowledge_Base.git
  ```

* ### 分支操作

  ```
  普通的查看分支操作:
  git branch
  
  查看远程分支操作
  git branch -r
  
  创建分支(注意分支名一定要见名思意)
  git branch new_branch_name
  
  切换分支
  git checkout new_branch_name
  
  切换并且创建分支
  git checkout -b new_branch_name
  ```

* ### 提交前的准备工作

  ```
  每次提交前先检查是否有代码更新，可以说管他有没有，都再次拉取一次
  
  两步的操作：
  git fetch  
  git merge
  
  或者说直接使用
  git pull
  ```

* ### 提交代码规范

  ```
  提交代码的时候，一定注意将 readme.md 和 其他文件的提交全部分开，不要都一起提交了
  
  对于 readme.md 的提交
  git add readme.md
  git commit -m "docs: update readme.md * n"    //  n 表示的是更新文档发次数
  git push -u origin new_branch_name
  
  
  其他文件的提交，可以每一个每一个的单独实现提交，还可以直接全部提交
  git add .
  git commit -m "commitlint规范: desc"
  git push -u origin new_branch_name
  ```


