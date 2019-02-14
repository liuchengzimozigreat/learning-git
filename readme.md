# this file is to record commands in learning git.

在git bash中切换硬盘分区，比如切换到H盘，你可以这样做——cd h:——，切换文件夹的操作和Linux无二。

some terms:<br>

术语 | 含义
--- | ---
**工作区/Working Directory:** | Directory you could see in your computer.
**版本库/Repository:** | A hidden directory in Working Directory including a stage, master, and Head--a pointer pointing to master, which could help us to reset our repository.
**暂存区/stage/index:** | "git add <file>" is actually adding <file> into stage<br>
**分支/master:** | "git commit -m "reminders"" is actually committing file to master.<br>

**1: git init**<br>
  initialize a git repository in a directory

**2: git add <file>**<br>
	add your file into workspace/stage controled by git
	you can add more than 1 file at once

**3: git commit -m "reminders/notices(提示信息)"**<br>
	commit files that you added in workspace/stage to the version repository--controled by git

**4: git status**<br>
	always use this command to see the current status
    untracked files: means a new file hasn't been added.

**5: git diff <file>**<br>
	help you check the differerce of between the <file> added into the stage and unstaged <file>

**6: git log / git log --pretty=oneline**<br>
	show the records of your previous activities.
	add "--pretty=oneline" would simplify the message and show the main information

**7: git reset --hard HEAD^/(commit id)**<br>
	make your repository go back to the last version/ the corresponding version of committing id

**8: git reflog**<br>
	show information of all the committing activities including committing ids and corresponding reminders/notices


**9: git clean -f**<br>
    delete all the untracked files in your Working Directory. Files not being added to the stage are all untracked.

**10: git diff HEAD -- <file>**<br>
    show the difference between <file> in Working Directory and HEAD in Repository

**11: git checkout -- <file>**<br>
    withdrawl all modifications in Working Directory.
    two situations:
    1: modified but not staged, then run this command, <file> will go back to the same status in Repository;
    2: staged but modified again, then run this command, <file> will go back to the same status in stage.

**12: git reset HEAD <file>**<br>
    withdrawl modification added into stage, then the <file> status became modified but unstaged.
    git reset <file>
    可以将暂存区（staged状态）（已经add但暂未提交的文件）文件扔回工作区（unstaged状态），然后再用11的方法，把修改撤销掉。







