learn git
//返回版本
git reset --hard commit_id
//返回前一个版本
git reset --hard HEAD^
//返回前两个
git reset --hard HEAD^
//返回前100
git reset --hard HEAD~100
穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。
要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。
//只修改没有没有add的message
no changes added to commit (use "git add" and/or "git commit -a")
