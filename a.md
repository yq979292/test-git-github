## 个人开发差用git
第一步 : 在需要git 管理的文件夹下打开git base here 
第二步：在git中进行项目管理的初始化 git init
第三步：在git中创建自己的项目文件
第四步：通过git add * 将所有的项目文件添加进去临时区域内
第五步：通过git commit -m 操作说明  将临时区域内的项目推送到本地的仓库上去
第六步：对项目进行修改之后,可以先看看修改了哪些东西，git diff 
第七步：确认完修改之后，可以通过git commit -a -m 操作说明 来进行上传了.
第八步：如果需要切换版本，只需要通过git reflog 查看下自己的操作历史，然后通过git reset 
--hard 版本号 就可以自由的切换不同的状态了。
第九步: 如需删除文件，使用git rm 文件名 来进行删除,然后通过git commit -a -m 提交
第十步:如果发生在本地误删的情况，可以直接使用git checkout 把临时区域的内容拉到本地

## 合作开发
1:创建本地ssh密钥；作用: 告诉远程仓库 是你自己推送的消息
~~~
$ ssh-keygen -t rsa -C "youremail@example.com"


查看生成的公钥
$ cat ~/.ssh/id_rsa.pub


ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCq8Z8JQgHpMZ3dRpULltEsnf5DEi95l1prLGjPE+q7qvNWc2GimWusIC/Pm4qY9RL2xJx1FUVfQW20wpuzBCldpJUv8eO7toJ1YKG0NqWajc1NfZLd+FixEXWeWvpyFD6VKdP33lLkgg3ixbZdyPLiAD56yo9JQPaaKBfxx2AD5pfn9JNw5S1QvznedZELyCMcRr95TNZVEFLEAhA32JcY19pAzmFZVzUfvIxBcZkjeNSAXxWO1eac+M4lhlHUrdeAZldru84SOaEOac68PinlD9yhKf2RaZIJwAYvoHkhqZGGwtqwSDEkTT2ahlTYSZGHB9IDYp3IgiSR+vD7zvWSEMBE/mmWWJnj3LaBdBvRUeXOLKb2xWa1nsDrZ5x2xwm33+OtTLm4l8WnoZp6Dyr1nQWSMN27ozZAgYdxCur+x1rthbHBm1gVs9kVnOuo70K9uvRj7LA4tkbTfRaHBWgBbJbt55mNitdMIiaDmbZybC2HxpLW7jUx40Kt/UQbjOc= 319281998@qq.com
~~~

第三部：在远程上新建密钥

