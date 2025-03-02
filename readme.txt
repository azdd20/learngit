Git is a distributed version control system.
Git is a very free software.
Git 命令必须在Git仓库目录执行，在仓库外执行是没有意义的
输入 git add readme.txt，得到错误 fatal:pathspec 'readme.txt' did not match any files.
添加某个文件是，该文件必须在当前目录下存在，用ls 或者dir查看当前目录的文件，查看文件是否存在
head 指向的版本就是当前版本。因此Git允许我们在版本的历史之间穿梭。使用命令git reset --hard commit_id
穿梭前，用git log 查看提交历史，以便确定要回到那个本本
要冲范围，用git reflog 查看历史命令，以便确定回到未来的那个版本
