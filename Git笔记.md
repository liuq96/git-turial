 #### Git相关笔记

1. 查看git相关版本
```
git --version
```

2. 配置用户名和邮箱
```
git config --global user.name ""
git config --global user.email ""
```

3. 配置常用Git命令别名
```
git config --global alias.st status
git config --global alias.ci commit
git config --global alias.co checkout
git config --global alias.br branch
```

4. 查看工作区
```
git rev-parse --git-dir
```

5. Git 配置
```
//版本库级别配置文件
git config -e
//全局配置文件
git config -e --global
//系统级别配置文件
git config -e --system
```

6. 退出Vim编辑方法
```
按住esc键，然后连续按大写模式下Z两次
```

7. 设置INI文件中的属性
```
git config <section>.<key> <value>
//比如更改用户名
git config user.name "newName"
```

8. 查看提交日志
```
git log --stat
```

9. 查看文件状态
```
//-s参数表示为精简输出
git status -s
```

10. add / commit关系
```
//将文件由工作区提交到暂存区
git add something 

//将文件由暂存区提交到版本区
git commit -m "tag"
```

11. diff命令
```
不带任何选项和参数调用git diff显示工作区和暂存区的差异

显示工作区和HEAD(当前工作区)的差异
git diff HEAD

通过参数--cached或--staged调用git diff显示暂存区和版本库的差异
git diff --cached
```

12. 不要使用git commit -a
```
虽然这个命令可以简化一些操作，减少git add命令的使用，但这么做相当于丢失了暂存区的作用，意味着丧失了对提交内容进行控制的能力。
```

13. git stash
```
当你想要切换分支，但又不想commit时，可以使用git stash来保存当前状态。
```