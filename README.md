# Git Alias 使用说明

> 本文档列出了我在日常开发中常用的 Git Alias 别名配置，现在分享给你，也希望对你有所帮助。

## ✨ 配置方式

1. 将 `git_alias.config` 文件复制到用户目录下（如 `~/.gitconfig`）。

2. 在终端中运行以下命令以应用别名：
    ```bash
    git config --global include.path ~/git_alias.config
    ```

## 📚 别名功能详解

别名 | 完整命令 | 用途说明
---|---|---
alias | git config --get-regexp alias | 查看所有已配置别名
st | git status | 显示变更和分支信息
co | git checkout | 切换分支或文件
sw | git switch | 推荐使用的新分支切换命令
br | git branch | 查看本地分支列表
new | git checkout -b | 创建并切换到新分支
aa | git add -A | 添加所有修改（包括删除）
cm | git commit -m | 以消息提交
last | git log -1 HEAD --stat --pretty=oneline | 查看最后一次提交详情
lo | git log --oneline --graph --decorate --all | 简洁图形化日志
ll | git log --pretty=fuller --stat | 详细提交记录
tidy |  | 删除本地已合并分支（保护 main/master/develop），带交互确认 
sync |  | 拉取最新代码并推送本地提交
unstage | git restore --staged | 撤销 git add 操作
undo |  | 清理未跟踪文件，恢复到最后一次提交状态
se | git grep -F | 在当前工作区搜索文本
wt | git worktree list | 查看所有工作树
wta | git worktree add | 新增工作树
wtd | git worktree remove | 移除工作树
visual | gitk --all | 可视化查看提交历史
fm | git fetch | 拉取远程更新


