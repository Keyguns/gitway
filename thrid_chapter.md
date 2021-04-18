## Create Project - get the basic to use git P25-P38 P42-P55
### 文档发生改变zsh中出现 黄叉
- 创建版本库
- 添加修改文件
- 创建分支
- 打标签并整理版本库
- 克隆版本库

- 创建版本库
>mkdir mysite  
>cd mysite  
>git init  
**版本库创建在文件夹中** .git
---
### **通过版本库记录和跟踪项目代码**
- 添加文件索引 (4.1)P42
>git add [filename] 
- 提交文件 **提交一次创建一个提交记录，标记代码演进** 一次可以提交多个提示信息
>git commit -m "commit message" [-m "commit message"]
>通过hash值唯一表示提交
- 显示提交日志
>git log [-num]

### 在项目中工作 处理文件修改
- 查看当前工作目录树状态 可以查看文件变化
>git status
### 理解并使用分支
- ***创建可选历史纪录*** 单纯commit不能回调版本
    1. 支持不同发布版本的分支
    2. 用来支持一个特定功能的开发的分支（Topic Branch）  
       为要发布的代码保留一份拷贝
    3. 新分支基于父分支
- 创建分支
>git branch new_branch_name  patent_branch_name
>git branch RB_1.0(realse branch) master
>给标签“打补丁”在标签处添加分支
>git branch new_branch_name tag_name
- 删除分支
>git branch -d [branch_name]
>删除末梢到最近标签的内容，**若重合仅为删除分支名**
- 切换分支
>git checkout branch_name

### 打标签
#### 用人类语言替代SHA
- 打标签 命令作用于全局
>git tag [tag_name] [分支末梢]
- 查看标签
>git tag
- 通过在标签处添加分支以用于切换过去
### 变基(合并) 将一条分支上的修改在另一条分支上重现
- 在需要合并的分支上使用
>当前分支>git rebase [be used branch_name]
### 通过标签名















