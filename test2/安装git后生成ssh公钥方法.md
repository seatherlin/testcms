### 安装git后生成ssh公钥方法



1，找到git的安装目录。在bin目录里面双击bash，会弹出窗口。

2，检查SSH keys是否存在：命令：ls -al ~/.ssh

3，生成新的ssh key：命令：

ssh-keygen -t rsa -C “1025408683@qq.com” 

其中：存储路径为C:\Users\Li Xiaohan\\.ssh\id_rsa

5，在c盘查看公钥。用记事本格式打开下述文件：C:\Users\Li Xiaohan\\.ssh\id_rsa.pub

生成的ssh公钥的格式是ssh-rsa开头的。

6，然后将ssh key添加到GitHub或者码云中。

————————————————
版权声明：本文为CSDN博主「天下熙熙皆为利来啊」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/qq_22182989/article/details/81429616





### 将代码链接到github远程库中：

```
echo "# testcms" >> README.md
git init
git add README.md
git commit -m "first commit"
# git branch -M main
git remote add origin git@github.com:seatherlin/testcms.git
git push -u origin main
```



参考文献：

https://blog.csdn.net/weixin_38317875/article/details/80925750