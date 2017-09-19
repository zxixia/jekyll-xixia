---
layout: post
title:  "Markdown语法笔记"
categories: Programmer
tags: Markdown
author: 西夏
description: 常用Markdown语法整理。
---

##  1，标题

Markdown的标题通过在行首插入`#`来实现，`#`的不同数量表示不同的标题级别，Markdown最多支持6级标题：

`# 一级标题`
# 一级标题

`## 二级标题`
## 二级标题

`### 三级标题`
### 三级标题

`#### 四级标题`
#### 四级标题

`##### 五级标题`
##### 五级标题

`###### 六级标题`
###### 六级标题

<br/>
## 2，换行
建议直接使用html标记`<br/>`，**`因为Markdown原生的方式只能换行，无法实现空出多行的效果`**。

<br/>
## 3，强调
### 3.1 斜体
用一对`*`扩起需要斜体的文本。
{% highlight shell %}
*需要斜体的文本*
{% endhighlight %}
*需要斜体的文本*。

<br/>
### 3.2 加粗
用一对`**`扩起需要加粗的文本。
{% highlight shell %}
**需要加粗的文本**
{% endhighlight %}
**需要加粗的文本**。

<br/>
### 3.3 加粗+斜体
用一对`***`扩起需要加粗的文本。
{% highlight shell %}
***需要加粗+斜体的文本***
{% endhighlight %}
***需要加粗+斜体的文本***。

<br/>
### 3.4 行内代码
用一对`` ` ``扩起需要行内代码的文本。
{% highlight shell %}
`需要行内代码的文本`
{% endhighlight %}
`需要行内代码的文本`。

<br/>
### 3.5 行内代码+斜体
用一对`*`嵌套`` ` ``扩起需要行内代码+斜体的文本。
{% highlight shell %}
*`需要行内代码+斜体的文本`*
{% endhighlight %}
*`需要行内代码+斜体的文本`*。

<br/>
### 3.6 行内代码+加粗
用一对`**`嵌套`` ` ``扩起需要行内代码+加粗的文本。
{% highlight shell %}
**`需要行内代码+加粗的文本`**
{% endhighlight %}
**`需要行内代码+加粗的文本`**。

<br/>
### 3.7 行内代码+加粗+斜体
用一对`***`嵌套`` ` ``扩起需要行内代码+加粗+斜体的文本。
{% highlight shell %}
***`需要行内代码+加粗+斜体的文本`***
{% endhighlight %}
***`需要行内代码+加粗+斜体的文本`***。


<br/>
## 4，分隔线
Markdown有如下三种画分隔线的方式：

```---```

---

```***```

***

`<hr/>`

<hr/>

<br/>
## 5，引用
### 5.1 单重引用
`>`用于表示引用。
{% highlight shell %}
>鲁迅说
>
>西夏很好！
{% endhighlight %}
>鲁迅说
>
>西夏很好！

<br/>
### 5.2 多重引用
`>`的不同数量表示不同的引用嵌套。
{% highlight shell %}
>鲁迅说
>
>西夏很好！
>>西夏也说
>>
>>西夏很Nice！
{% endhighlight %}
>鲁迅说
>
>西夏很好！
>>西夏也说
>>
>>西夏很Nice！


<br/>
## 6，链接
### 6.1 直接链接
{% highlight shell %}
[西夏](http://xixia.info/)
{% endhighlight %}
[西夏](http://xixia.info/)

<br/>
### 6.2 间接链接
{% highlight shell %}
[西夏][xixia]

[xixia]:http://xixia.info/
{% endhighlight %}
[西夏][xixia]

[xixia]:http://xixia.info/


<br/>
## 7，图片
### 7.1 直接图片
{% highlight shell %}
![西夏](http://xixia.info/assets/images/xixia.gif)
{% endhighlight %}
![西夏](http://xixia.info/assets/images/xixia.gif)

<br/>
### 7.2 间接图片
{% highlight shell %}
![西夏][xixia_pic]

[xixia_pic]:http://xixia.info/assets/images/xixia.gif
{% endhighlight %}
![西夏][xixia_pic]

[xixia_pic]:http://xixia.info/assets/images/xixia.gif


<!-- 后面是文章参考资料 -->
<br/>
### 参考资料：

1，[Markdown 语法说明 (简体中文版)][markdown-appinn]

2，[markdown 转义][csdn-ISaiSai]

3，[markdown简明语法][cnblogs-back_man]

4，[markdown学习笔记][jianshu-wo-niu]

<!-- 文章插图和超链接 -->
[markdown-appinn]: http://www.appinn.com/markdown/
[csdn-ISaiSai]: http://blog.csdn.net/isaisai/article/details/51513116
[cnblogs-back_man]: http://www.cnblogs.com/back-man/p/5012746.html
[jianshu-wo-niu]: http://www.jianshu.com/p/4Q3aay
