git init

git add XXX

git commit -m "XXX"


git log
git log XXX
git log --pretty=oneline

git diff


git status


git reset --hard HEAD^			回退到上一版本
git reset --hard HEAD^^			回退到上上次版本
git reset --hard HEAD~100		回退到第100 次时的版本
git reset --hard XXX			回退到指定版本

git reflog				显示每一次的提交/回退指令


git checkout -- XXX			回退文件到最近一次 commit 或 git add 的状态

git reset HEAD XXX			将暂存区中的文件撤销掉（从暂存区中删除该文件的修改记录）

git rm XXX				从 git 库中删除 XXX 文件

// git 分支
git branch				查看 git 分支
git branch XXX				创建分支·
git branch -d XXX			删除某一个分支
git checkout -b XXX			新建并切换分支
git checkout XXX			切换分支
git merge XXX				将某分支合并到 master 分支·


git log --graph				查看分支合并图
	eg:  git log --graph --pretty=oneline --abbrev-commit

ssh-keygen -t rsa -C "youremail@example.com"	创建SSH Key

git merge dev				把dev 分支合并到当前分支
git merge --no-ff -m "xxx" dev		把dev 分支合并到当前分支，并创建新的 commit


git stash				将当前的修改 stash 起来，stash 之前，本分支的修改将会不可见，可以在 stash 之后，修改其他分支的 bug
git stash list				显示 stash 列表
// 恢复 stash 的内容
git stash apply stash@{index}
git stash pop

git stash drop				删除某一个 stash

// 重命名文件或文件夹
git mv -f old new
git add -u newfolder (-u选项会更新已经追踪的文件和文件夹)

