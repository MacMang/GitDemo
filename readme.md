1. git init (只需要初始化一次)
2. git add .或* 或 文件名.后缀
    .: 表示将被修改的文件存入暂存区域
    *: 所有文件都存入到暂存区域
    文件名.后缀： 直接指定文件
3. git commit -m "提交的描述" （将记录提交到git仓库里，就是隐藏掉的哪个git目录）

4. git 状态
    已修改  
    已暂存
    已提交
5. git log 查看历史版本
    commit 1f228fc6d0e32e1ad45bb2b76e7929173e46abfb (HEAD -> master)
    Author: zmt <mt@qq.com>
    Date:   Fri Jul 19 10:32:40 2019 +0800

6. 回溯历史版本
    git reset --hard hash值

7. 简化log信息
    将版本信息显示在一行内

8. 将文件从暂存区域和工作目录一起删除
    git rm -f 文件名.后缀
    如果已经在工作目录中删除了文件，但是在暂存区域里还是存在该文件
    则需要通过 该命令进行删除操作

9. 只删除暂存区域内的文件，不删除工作目录文件
    git rm --cached 文件名.后缀

