# XDU-Wiki
## 项目介绍
欢迎访问XDU-WiKi！，本项目旨在整合XDU内部的校园资源，为西电的学生们提供生活和学习上的指导，欢迎任何同学PR~  
项目网站地址:https://insightsxdu.github.io/XDU-WiKi/

## 项目规划
项目的初衷是为了帮助在西电就读的本科生们，为他们提供一个完善合理与时俱进的学习路线以及指导框架

## 如何贡献？
我们欢迎更多的同学对该repo有更多建议和优化方案，欢迎您使用`Forking`工作流提交 Pull Request，具体参考[atlassian文档](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)，大致步骤如下：

1. 在GitHub上Fork本仓库
2. Clone Fork后的个人仓库
3. 设置`upstream`仓库地址，并禁用`push`
4. 我们建议使用分支开发
5. PR之前保持与原始仓库的同步，之后发起PR请求
6. PR通过后，我们会将您的PR合并到主分支中

命令示例
```bash
# fork
# clone forked repo
git clone git@github.com:USERNAME/XDU-WiKi.git

# set upstream
git remote add upstream git@github.com:InsightsXDU/XDU-WiKi.git
# disable upstream push
git remote set-url --push upstream DISABLE
# verify
git remote -v
# origin  git@github.com:NoFish-528/XDU-WiKi.git (fetch)
# origin  git@github.com:NoFish-528/XDU-WiKi.git (push)
# upstream        git@github.com:InsightsXDU/XDU-WiKi.git (fetch)
# upstream        DISABLE (push)

# 新建分支<可选>，并切换到该分支
git checkout -b <branch_name>
# edit and commit and push your changes
git push -u origin <branch_name>

# 以下内容均可选，但建议执行
# keep your fork up to date
## fetch upstream main and merge with forked main branch
git fetch upstream
git checkout main
git merge upstream/main
## rebase brach and force push
git checkout <branch_name>
git rebase main
git push -f
```
# 贡献内容示范
本项目基于mkdocs构建完成，当您fork到本地后，如果想要贡献内容，请在XDU-WiKi/doc/对应模块 内容下修改或增加您想贡献的内容，之后在XDU-WiKi/mkdocs.yml配置文件中修改对应的目录，当PR并入后效果就将呈现在在线网站上。  
## 示例如下：
当我想要在开始界面中增加自我介绍文件：  

1. fork仓库至我的仓库中  
2. 克隆该仓库
3. 在本地打开该仓库
4. 增加docs/开始/自我介绍.md  
5. 修改对应的mkdocs.yml文件中内容，同时在docs/参与贡献/项目结构.md中修改对应内容  
**原文件**
```yml
nav:
    - 开始:
          - 欢迎: index.md
          - 路线分享: 
              - 序言: 开始/路线分享序言.md
    - 生活: 
          - 序言: 生活/序言.md
    - 在校学习指南:
          - 基础学科: 在校学习指南/基础学科/序言.md
          - CV方向: 在校学习指南/CV方向/序言.md
          - NLP方向: 在校学习指南/NLP方向/序言.md
          - 前端: 在校学习指南/前端/序言.md
          - 后端: 
              - 序言: 在校学习指南/后端/序言.md
    - 社团与工作室们: 
          - 序言: 社团与工作室们/序言.md
    - 保研: 
          - 序言: 保研/序言.md
    - 考研: 
          - 序言: 考研/序言.md
    - 工作: 
          - 序言: 工作/序言.md
    - 参与贡献:
          - 如何贡献: 参与贡献/如何贡献.md
          - 项目结构: 参与贡献/项目结构.md
    - 关于 Datawhale: https://datawhale.club/

```  
**修改后**
```yml
nav:
    - 开始:
          - 欢迎: index.md
          - 路线分享: 
              - 序言: 开始/路线分享序言.md
    - 生活: 
          - 序言: 生活/序言.md
    - 在校学习指南:
          - 基础学科: 在校学习指南/基础学科/序言.md
          - CV方向: 在校学习指南/CV方向/序言.md
          - NLP方向: 在校学习指南/NLP方向/序言.md
          - 前端: 在校学习指南/前端/序言.md
          - 后端: 
              - 序言: 在校学习指南/后端/序言.md
    - 社团与工作室们: 
          - 序言: 社团与工作室们/序言.md
    - 保研: 
          - 序言: 保研/序言.md
    - 考研: 
          - 序言: 考研/序言.md
    - 工作: 
          - 序言: 工作/序言.md
    - 参与贡献:
          - 如何贡献: 参与贡献/如何贡献.md
          - 项目结构: 参与贡献/项目结构.md
    - 关于 Datawhale: https://datawhale.club/
```  

6. 提出PR等待并入
7. PR合并后查看在线网页更新内容

贡献内容中，请您在您贡献的标题页下加入您的姓名  
形式如下：  
标题  
author:xxx  
**感谢您的贡献！**
## Contributors
<a href="https://github.com/InsightsXDU/XDU-WiKi/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=InsightsXDU/XDU-WiKi" />
</a>

Made with [contrib.rocks](https://contrib.rocks).