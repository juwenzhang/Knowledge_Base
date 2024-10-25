## 该仓库介绍

* 该仓库使用来实现的是将所有的学习的部分按照不同的分支进行存储的一个仓库

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

  