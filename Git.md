# Github学习
1. 创建版本库

   `sudo apt-get install git`

   ```
   mkdir <learngit>
   cd <learngit>
   pwd
   git init
   ```
   ```
   git add <file>暂存区
   git commit -m "<message>"
   ```
2. 时光机穿梭

   ```
   git status
   git diff
   git log --pretty=oneline
   git reset --hard HEAD^
   git reset --hard <commit-id>
   git reflog
   ```
   ```
   撤销修改
   工作区：git checkout --<file>
   暂存区：git reset HEAD <file>
          git  checkout --<file>
   版本库：版本回退  
   ```  
   ```
   删除文件
   git rm <file>
   git commit -m "message"确认删除
   git checkout --<file>误删恢复
3. 远程库管理

   ```
   ssh-keygen -t rsa -C "<youremail@example.com>"
   在主目录下ctrl+h找到.ssh文件中打id_rsa.pub，粘贴公钥
   ```
   ```
   git push -u origin master
   git push origin master
   ```
   ```
   git clone git@github.com:enlighten0707/<reponame>.git
   ```
4. 分支管理
   ```
   git branch -b dev
   git branch
   git add
   git commit
   git checkout master
   git merge dev
   git branch -d dev
   git log --graph --pretty=oneline
   git merge --no-ff -m "merge with no-ff" dev
   ```
   ```
   git stash
   git stash list
   git stash pop
   ```
   ```
   git remote
   git remote -v
   git checkout -b dev origin/dev
   git pull
   ```
   `git rebase (?)`
5. 标签管理
   ```
   git tag v1.0
   git tag

   git log
   git tag v0.9 <commit-id>

   git show v0.9
   git tag -a v0.9 -m "" <commmit-id>

   git tag -d v0.1
   git push origin v1.0
   git push origin --tags
   git push origin :refs/tags/v0.9
   
   ```



