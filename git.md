# git小记

---

## 命令:

1. 配置命令别名 `git config --system alias.{short name} {origin name}`
2. 列出所有别名配置 `git config --get-regexp alias`
3. 打标签
- 轻量级标签 `git tag {tagname}`
- 含附注标签 `git tag -a {tagname} -m {annotation}`
- 推送分支 `git push origin {tagname}`
- 推送所有分支 `git push origin --tags`

4. 重命名分支
- 命名任何一个分支 `git branch -m {oldname} {newname}`
- 命名当前分支 `git branch -m {newname}`

5. 删除文件
- 从仓库中以及从文件系统中删除文件: `git rm {file name}`
- 仅从仓库中删除文件: `git rm --cached {file name}`

## 配置相关
- 列出所有别名: git config --get-regexp alias

## 问题
1. `git status` 乱码 `git config --global core.quotepath false`