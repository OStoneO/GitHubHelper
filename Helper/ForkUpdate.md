更新自己Fork的代码
==
以GitHub用户OStoneO为例子，在你操作的时候要把下面的GitHub用户名OStoneO换成你自己的GitHub用户名：

注意事项：在更新自己Fork的代码之前，需要先把自己在本地的更改进行提交。

### 1、检出自己在GitHub上fork的JQuery分支

git clone https://github.com/OStoneO/jquery.git

cd jquery

` 如果已经检出了代码，则此步骤为切换到jquery根目录然后执行第二步 `

### 2、增加JQuery的远程原始分支（用户JQuery的分支）到本地

` 如果以前已经执行过本操作，则可忽略，当然，需要用git remote -v命令里确认是否有jquery-OStoneO分支 `

git remote add jquery-OStoneO https://github.com/jquery/jquery.git

运行命令：git remote -v你会发现多出来了一个jquery-OStoneO的远程分支。如下： 
```
jquery-OStoneO     https://github.com/jquery/jquery.git (fetch)

jquery-OStoneO     https://github.com/jquery/jquery.git (push)

origin  https://github.com/OStoneO/jquery.git (fetch)

origin  https://github.com/OStoneO/jquery.git (push)
```
### 3、把远程原始分支jquery-OStoneO的代码拉到本地

git fetch jquery-OStoneO
### 4、合并对方远程原始分支jquery-OStoneO的代码

git merge jquery-OStoneO/master
### 5、把最新的代码推送到你的GitHub上

git push origin master

### 6、发送Pull Request到jquery-OStoneO

用自己的GitHub账号登陆GitHub网站

打开https://github.com/OStoneO/jquery

点击Pull Request

点击New Pull Request

输入Title简要描述你改进的功能

输入详细的功能说明

点击Send pull request

这样就把你的所有commit发送给jquery-OStoneO了

### 7、指令示例

克隆指定分支版本到指定文件加
```
git clone https://github.com/OStoneO/jquery.git ./jquery_1.12/ -b 1.12-stable
```

copy from [here](https://github.com/ysc/APDPlat/wiki/%E5%A6%82%E4%BD%95%E6%9B%B4%E6%96%B0%E8%87%AA%E5%B7%B1Fork%E7%9A%84%E4%BB%A3%E7%A0%81)

`changed by myself`
