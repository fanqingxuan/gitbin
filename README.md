### 进一步精简git命令

### 背景&目标

熟悉git命令的小伙伴对于git add、git pull、git push、git commit、git checkout命令应该不陌生了，大家有没有发现每一个命令我必须输入git + 命令，好麻烦啊，此项目正式为了解决这个问题，git add 改成add,git pull 改成 pull,push代替了git push。**完全告别前面的git三个单词**，可选参数完全兼容git的原有参数


### 支持命令

| 命令 | 对应git命令 |
| ------- | ------- |
|    add     | git add        |
|    commit     | git commit        |
|    checkout     | git checkout        |
|    branch     | git branch        |
|    br     | git branch        |
|    cherry-pick     | git cherry-pick        |
|    st     | git status        |
|    status     | git status        |
|    log     | git log        |
|    gll     | git log --graph --all --pretty=format:'%Cred%h %Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative        |
|    greset     | git reset        |
|    gdiff     | git diff        |
|    rebase     | git rebase        |
|    stash     | git stash        |
|    merge     | git merge        |
|    pull     | git pull        |
|    push     | git push        |


### 示例
```
add -u # 修改的内容提交到暂存区
branch -D test # 删除test分支
commit -m "this is commit" #将暂存区代码提交到仓库
push #推送到远端
```

### 注意事项
- ll命令容易跟linux的ls别名命令ll冲突，所以用gll命令作为git ll命令
- greset命令等价于git reset
- diff命令是linux的命令，为防止冲突用gdiff命令作为git diff的快捷命令

### 安装方式

- 第一步:clone仓库代码到本地
```bash
https://github.com/fanqingxuan/gitbin.git
```
- 第二步:将仓库的bin目录设置到path环境变量

- 第三步:如果是windows用户，需要关闭dos终端，重新打开终端

### 其它
支持windows&linux操作系统
