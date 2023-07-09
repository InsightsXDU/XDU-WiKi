# XDU-Wiki
## 项目介绍
欢迎访问XDU-WiKi！，本项目旨在整合XDU内部的校园资源，为西电的学生们提供生活和学习上的指导，欢迎任何同学PR~  
项目网站地址:https://limafang.github.io/XDU-WiKi/

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

## Contributors
<a href="https://github.com/InsightsXDU/XDU-WiKi/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=InsightsXDU/XDU-WiKi" />
</a>

Made with [contrib.rocks](https://contrib.rocks).