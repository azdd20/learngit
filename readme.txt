Git is a distributed version control system.
Git is a very free software.
Git 命令必须在Git仓库目录执行，在仓库外执行是没有意义的
输入 git add readme.txt，得到错误 fatal:pathspec 'readme.txt' did not match any files.
添加某个文件是，该文件必须在当前目录下存在，用ls 或者dir查看当前目录的文件，查看文件是否存在
head 指向的版本就是当前版本。因此Git允许我们在版本的历史之间穿梭。使用命令git reset --hard commit_id
穿梭前，用git log 查看提交历史，以便确定要回到那个本本
要冲范围，用git reflog 查看历史命令，以便确定回到未来的那个版本
当该乱了工作区某个文件的内容，想直接丢弃工作区的修改，用命令git cehckout --file
当不但改乱了工作区某个文件的内容，还添加到了暂存区，，像丢弃修改，分两步，第一不用指令 git reset head <file> ，就回到了上一行
git rm 用于删除一个文件。如果一个文件已被提交到版本库，那么永远不用担心被误删，但是只能恢复文件到最新版本，会丢失最近一次提交后修改的内容。
要关联一个远程库，使用命令 git remote add origin git@server-name:path reponame.git
关联一个远程库是必须给远程库指定一个名字，origing是默认习惯明明；
关联后，使用命令git push -u origing master 第一次推送 master 分支的所有内容；
关联后，使用命令git push -u origing master 第一次推送 master 分支的所有内容
每次本地提交后，只要有必要，就可以使用命令git push origing master 推送最新修改

要克隆一个仓库，首先必须知道一个仓库的地址,然后使用git clone 命令克隆
git 支持多种协议，包括https,但ssh协议速度最快
it is my pleasant