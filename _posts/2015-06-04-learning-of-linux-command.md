---
layout: post
title:  "linux 命令学习笔记一"
date:   2015-06-04
description: linux 命令学习   
keywords: linux command learning
---
<h5>1、新建用户</h5>
<!-- 高亮显示背景，用于标识代码块 -->
{% highlight ruby %}
$ useradd [options] uername	
$ adduser username
{% endhighlight %}
<section>
	注：这两个命令都可以创建新用户，adduser会自动完成新用户的基本设置，所以adduser较适合初学者使用;<br>
useradd命令参数：<br>	
  	<img src="{{ site.baseurl }}/images/study/useradd.png" alt="useradd command">
  	<br>
  	如：<br>
  	<pre>
$ useradd -d me	//则会新建一个me用户，并会在home目录下建立一个me目录，作为用户me的主目录

$ passwd me	
//为用户me设置密码，执行这个命令需要root权限，可以切换到root或在命令前加 suod（表示以超级用户身份执行）
  	</pre> 
</section>
<h5>2、显示当前用户</h5>
<pre>$ who am i</pre>
<h5>3、删除/切换 用户</h5>
<pre>
$ userdel -r username
$ su username
</pre>
<h4>网络类</h4>
<h5>查看网络信息</h5>
<pre>$ ifconfig [options]</pre>
<h5>设置ip</h5>
<pre>$ ifconfig eth0 youripaddress netmask yourmask</pre>
<h5>关闭防火墙</h5>
<pre>$ iptables -F</pre>

<!-- 引用图片 -->
<!-- <img src="{{ site.baseurl }}/images/red.png" alt=""> -->