# git使用笔记
  主要用于记录，下次忘记如何用时，不用去百度
  ## 1.如果电脑上第一次安装使用，先配置
       1.1 创建本地ssh key（需要添加到github中）
       ssh-keygen -t rsa -C "github注册的邮箱"
       一直回车就可以
       1.2 将生成的文件 id_rsa.pub复制，然后在自己的github远程端的settings中的ssh and GPG keys中添加一个ssh keys，在keys中粘贴刚刚复制的内容。
       1.3检测是否成功，在git客户端输入 ssh -T git@github.com ，如果看到最后一行是 Hi owlsignl! You've successfully authenticated, but GitHub does not provide shell access.则表示成功
       1.4 设置自己的username和useremail,git会将信息记录，不然每次commit时都会提示登录
          git config --global user.name "github上的name"
          git config --global user.email "github注册的邮箱"


