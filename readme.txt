learn git
//设置git的name和email（全局）
git config --global --user.name "yourname"
git config --global --user.email "youremail"
//创建目录 选择目录
mkdir learnGit
cd learnGit
//显示当前路径
pwd
//初始化当前目录为仓库
git init

//返回版本
git reset --hard commit_id
//返回前一个版本
git reset --hard HEAD^
//返回前两个
git reset --hard HEAD^^
//返回前100
git reset --hard HEAD~100
穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。
要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。
//只修改没有没有add的message
no changes added to commit (use "git add" and/or "git commit -a")
// * branch            master     -> FETCH_HEAD
//fatal: refusing to merge unrelated histories
//错误提示如下原因是在本地的文件夹为NewRepo，与远程仓库名称不一样
//解决方案:pull时添加–-allow-unrelated-histories
$ git pull --allow-unrelated-histories
//merge 将分支merge到现在的分支上
git merge <branch>