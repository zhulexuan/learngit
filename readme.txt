git init : 启动！
git add : 加入暂存区
git commit -m "file name" : 提交，存档
git status : 查看状态。
git diff "file name" : 比较工作区和暂存区的差异。 
git log : 查看当前版本的祖先版本信息。
git reflog : 查看所有版本。
git reset --hard HEAD^ : 重置为上一个版本的已提交状态，其中HEAD后的"^"可增加，对应回退的步数。
git reset --hard HEAD~*** : 回退 *** 步，"***"为一个具体的数字。
git reset --hard eaadf4e38... : 重置为 eaadf4e38... 对应版本，“eaadf4e38...”是版本编号。
git reflog : 查询每一次命令（可用来找版本号）
git checkout -- "file name" : 撤销file在工作区内的全部修改，误删文件可以恢复。
git reset HEAD "file name" : 把暂存区的修改撤销，放回工作区。
git rm "file name" : 彻底删除一个文件（删除文件，并从版本库内移除）。
ssh-keygen -t rsa -C "youremail@example.com" : 创建一个钥匙，“”内的是钥匙的备注信息（名字）。
github - Create a new repo : 创建新远程仓库，并填入名字。
git remote add origin git@github.com:michaelliao/learngit.git : 本地关联远程库，其中":"后的内容需要对应修改。
git push -u origin master : 把本地的仓库推送到远程（第一次时使用）。
git push origin master : 后续使用。
git remote -v : 查看远程库信息。
git remote rm “name” : 解除本地和远程的绑定关系，“name”为远程库名字，如origin。
git clone git@github.com:michaelliao/gitskills.git : 将github上的库克隆到本地，会在当前目录下建立对应子目录。
git branch : 查看所有本地分支。
git branch "name" : 创建分支name。
git switch "name" : 切换到分支name。
git merge "name" : 将分支name合并到当前分支中。
git branch -d "name" : 将分支name删除。
git switch -c "name" : 创建并切换到分支name。
git merge --no-ff -m "message" "name" : 禁用Fast forward的合并，会记录合并对应的分支过程。
分支策略：master作为大版本器记录（递交评测），dev是工作主线（小优化），具体在详细分支上改动。

