#git command

git init，初始化，表示即将对当前文件夹进行版本控制。
git status，查看Git当前状态，如：那些文件被修改过、那些文件还未提交到版本库等。
git add 文件名，将指定文件添加到版本库的暂存状态。
git commit -m '提交信息'，将暂存区的文件提交到版本库的分支。
git log，查看提交记录，即：历史版本记录
加参数  --pretty=oneline，只会显示版本号和提交时的备注信息

#回滚到指定版本：
git log 查看提交记录
git rest --hard commit-id

git reflog  可以查看所有分支的所有操作记录（包括已经被删除的 commit 记录和 reset 的操作）

git reflog -n  后面跟数字，可以显示指定数字的行


