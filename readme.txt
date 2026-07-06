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
