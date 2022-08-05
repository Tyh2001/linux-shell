# Linux-shell

## 基本命令

```shell
ssh name@ip # 登陆服务器

cd xxx # 进入指定目录

cd .. # 退到上一层目录

cd / # 进入主目录

sudo -i # 切换 root 用户

rm -rf xxx/* # 删除 xxx 目录中的所有文件

mkdir xxx # 新建文件夹

touch xxx # 新建文件

vim xxx # 编辑文件

vi xxx # 编辑文件

cat xxx # 查看文件内容

ll # 查看当前目录所有文件
```

## 错误处理

- 错误 1

```shell
-bash: ./tyh-blog.sh: Permission denied
```

需要添加上可执行权限，执行命令：

```shell
chmod 777 xxx.sh
```

- 错误 2

```shell
rm: cannot remove 'blog/.user.ini': Operation not permitted
```

执行下面命令再删除：

```shell
chattr -i .user.ini
```
