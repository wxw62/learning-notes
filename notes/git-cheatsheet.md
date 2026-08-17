# Git 速查

## 日常流程

```bash
git status                 # 查看工作区状态
git add -A                 # 暂存所有改动
git commit -m "message"    # 提交
git push                   # 推送
git pull --rebase          # 拉取并变基
```

## 分支操作

```bash
git branch -a              # 列出所有分支
git checkout -b feature    # 新建并切换分支
git merge feature          # 合并分支
git branch -d feature      # 删除已合并分支
```

## 撤销

```bash
git restore <file>         # 丢弃工作区改动
git restore --staged <f>   # 取消暂存
git reset --soft HEAD~1    # 撤销提交但保留改动
git reset --hard HEAD~1    # 彻底回退（慎用）
```

## 查看历史

```bash
git log --oneline --graph --all
git log -p                 # 带 diff 的历史
git blame <file>           # 每行是谁改的
```
