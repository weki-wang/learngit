# git学习

## 基本操作

1. git 的工作原理如下：
   
     工作区  --->  储藏区  ----> 本地仓库  ---> 远程仓库
   
     其中：
   - 工作区 ---> 储藏区 : `git add -- filename`  
   - 储藏区 ---> 工作区 : `git reset -- filename`   
   - 储藏区 ---> 本地仓库 : `git commit -m "message"`
   - 本地仓库 ： 提交到了本地仓库后，只能进行版本回退
   
   

2. 撤销修改：

   - 如果在工作区进行了修改，没有提交到储藏区 : `git checkout -- filename`
   - 如果在工作区修改了，并且提交到储藏区：
        - 先撤回到工作区 : `git reset -- filename`
        - 然后撤销修改: `git checkout -- filename`



3.  删除 ：
  
   - 删除本地仓库的内容 ：`git rm -- filename` 



4. 版本退回：
   - 版本退回命令 : `git reset --hard xxxxx`
   - 查看退回历史以及未来的提交 ： `git reflog`

