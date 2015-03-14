---
layout: post
title:  "ubuntu git.oschiane.net 配置"
date:   2015-03-13 12:54
categories: git
---

### ssh配置

{% highlight ruby %}
1. ssh-keygen -t rsa -C "gyxllxw5201@126.com" 

生成密钥时,会让用户选择存储目录,按照默认的提示保存,不要修改路径,否则后面测试会不通过

2. 将public key 添加到 服务器 git@osc http://git.oschina.net/keys

cat ~/.ssh/id_rsa.pub

3. 终端测试: ssh -T git@git.oschina.net 

若返回 Welcome to Git@OSC, your name 则证明添加成功

{% endhighlight %}
