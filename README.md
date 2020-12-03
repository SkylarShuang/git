# git 学习笔记

<mark>HAED</mark>表示当前版本，<mark>HAED^</mark> 表示上一个版本，<mark>HAED^^</mark>表示上上版本，<mark>HAED~100</mark>表示上一百个版本

**git reflog**  查看命令历史

**git merge** 命令合并指定分支和当前分支

通常合并（merge）分支时，会采用Fast forward模式，如下图。在这种模式下，删除分支后，会丢掉合并该分支的信息（类似于无痕？？）。

<u>合并前</u>
![Screenshot 2020-12-03 at 3.23.06 PM](/Users/80303015/Library/Application Support/typora-user-images/Screenshot 2020-12-03 at 3.23.06 PM.png)

<u>*合并后*</u>
![Screenshot 2020-12-03 at 3.23.06 PM-6981894](/Users/80303015/Library/Application Support/typora-user-images/Screenshot 2020-12-03 at 3.23.06 PM-6981894.png)

如果强制禁用Fast forward模式，git会在merge的时候生成一个新的commit信息，这样就可以在历史记录找到合并分支的信息

