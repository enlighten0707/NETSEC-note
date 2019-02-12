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


