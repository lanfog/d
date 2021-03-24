Markdown语法介绍
===
Markdown的目的在于“易读易写”
易读：让你的文章层次清楚，版面清晰；
易写：使你能够在写完代码的同时就已经排好版了。
接下来为一个简单的markdown语法介绍

## 一、标题

大标题  
===================================  
  大标题一般显示最上方的主标题,类似html的\<h1\> 
  你只要在标题下面跟上=====即可  
    
中标题  
---
  中标题一般显示重点项,类似html的\<h2\>  
  你只要在标题下面输入-----即可  
    
### 小标题  

  小标题类似html的\<h3\>  
  小标题的格式如下 ### 小标题   
   
### `说明`:
  
  1. #和===，##和---是一样的效果<br>
  2. #和标题字符中间要有空格  
  3. 一个到六个#对应\<h1\>到\<h6\> 
  
## 二、段落

### 代码段
  
#### 比如我们可以在多行文本框里输入一段代码,来一个Java版本的HelloWorld吧  

    public class HelloWorld {  
      /**  
      * @param args  
      */  
      public static void main(String[] args) {  
      System.out.println(“HelloWorld!”);  
    }  

### 文本段

#### 文字被某些字符包围
> 文字被些字符包围  
>  
> 只要在文字前面加上>空格即可  
>  
> 如果你要换行的话,新起一行,输入>空格即可,后面不接文字  
> 但> 只能放在行首才有效  
  
#### 文字被某些字符包围,多重包围  
> 文字被些字符包围开始  
>  
> > 只要再文字前面加上>空格即可  
>  
>  > > 如果你要换行的话,新起一行,输入>空格即可,后面不接文字  
>  
> > > > 但> 只能放在行首才有效  

### 列表

#### 有序列表

1. 第一条
2. 第二条
3. 第三条

数字接着一个英文句点作为有序列表标记

#### 无序列表

* 第一条
* 第二条
* 第三条

使用*，-或者+作为无序列表的标记

### `说明`:
  1、默认段落前后各需留一个空行，否则不换行；<br>
  2、需要手动换行则可以使用\<br\>，或者在句尾打两个空格；<br>
  3、有序列表英文句点后需要一个空格。<br>

## 三、特殊文本

### 链接  

[点击这里你可以链接到www.oschina.net](http://www.oschina.net)<br />  
  
### 图片  
![baidu](http://www.oschina.net/img/logo_s2.png)  
  
### 想点击某个图片进入一个网页,比如我想点击下面的logo然后再进入www.oschina.net  
[![image]](http://www.oschina.net/)  
[image]: http://www.oschina.net/img/logo_s2.png  

### 强调

两个星号里面的文字会被**加粗**

用**或者__包起来的文字能使其加粗

### 代码

Use `printf()` function

可以用（`）把句子中的小段代码包括起来

```
public class HelloWrold{
  public tatic void main(String args[]){
      System.out.println("hello,world");
  }
}
```

可以用（```）把代码段包括起来
## 四、表格

```
|综合资讯|软件更新资讯|
|----|----|
|IoTivity —— 开源物联网软件框架和服务|SeaMonkey 2.32 发布，Firefox 浏览器套件|
|Git@OSC 项目推荐 —— OpenDroid ORM 框架|fastjson 1.2.4 发布，Java 的 JSON 开发包|
|2015 年最好用的企业级 Linux 开源软件|Apache Commons Validator 1.4.1 发布|
|【每日一博】Redis 脚本实现分布式锁|Smack 4.1.0-beta1 发布，XMPP 开发包|
```

|综合资讯|软件更新资讯|
|----|----|
|IoTivity —— 开源物联网软件框架和服务|SeaMonkey 2.32 发布，Firefox 浏览器套件|
|Git@OSC 项目推荐 —— OpenDroid ORM 框架|fastjson 1.2.4 发布，Java 的 JSON 开发包|
|2015 年最好用的企业级 Linux 开源软件|Apache Commons Validator 1.4.1 发布|
|【每日一博】Redis 脚本实现分布式锁|Smack 4.1.0-beta1 发布，XMPP 开发包|
## 五、其他

### 特殊字符处理  
有一些特殊字符如<,#等,只要在特殊字符前面加上转义字符\即可<br />  
你想换行的话其实可以直接用html标签\<br/\>  

### 自动链接

markdown能把用<>包括起来的短地址自动转化成链接
<www.oschina.net>

<br>

### 删除线

使用两个~~包括文字，文字将显示删除样式，

如 ~~这是被删除的文字~~

更多详细资料可以参考 <http://wowubuntu.com/markdown/>