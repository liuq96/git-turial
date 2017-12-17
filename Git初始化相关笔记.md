#### Git初始化相关笔记

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

