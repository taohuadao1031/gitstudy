#git command

git init，初始化，表示即将对当前文件夹进行版本控制。
git status，查看Git当前状态，如：那些文件被修改过、那些文件还未提交到版本库等。
git add 文件名，将指定文件添加到版本库的暂存状态。
Git 2.x 之后版本，以下2个命令都可以把所有的文件添加到暂存区。
git add .	
git add --all

git commit -m '提交信息'，将暂存区的文件提交到版本库的分支。
git log	查看所有提交过的记录，即：历史版本记录
加参数 --pretty=oneline，只显示版本号和提交时的备注信息
加参数 --oneline	显示精简的版本号和提交的备注信息
加参数 -n  后面跟数字，可以显示指定数字最近的commit记录

查找某位作者提交的commit:
git log --oneline --author="name"

查找commit信息里指定的内容
git log --oneline --grep="commit"

查找某个时间段提交的
git log --oneline --since="9am" --until="12am"

查找历史提交的记录，2019年9月25日之后，每天早9点12点提交的commit
git log --oneline --since="9am" --until="12am" --after="2019-09-25"



#回滚到指定版本：
git log 
git rest --hard commit-id

git reflog  可以查看所有分支的所有操作记录（包括已经被删除的 commit 记录和 reset 的操作）

git reflog -n  后面跟数字，可以显示指定数字的行
