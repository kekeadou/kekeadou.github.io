---
layout: post
title: vim插件学习
category: itbasic
tags: []
---
##  emmet:  
C+Y 为引导键。  
  
, 将css语法的选择器扩展为html文本。  
比如, div#page>ul.foo*3，按下C+Y , 就会被扩展为：  
<div id="page">  
    <ul class="foo1"></ul>  
    <ul class="foo2"></ul>  
    <ul class="foo3"></ul>  
</div>  
  
还有一种用法，  
test1  
test2  
test3  
全选中以后，按下C+Y ,在命令栏会提示Tag：，输入ul>li.foo*,会变为：  
    <ul>  
        <li class="foo1">test1</li>  
        <li class="foo2">test2</li>  
        <li class="foo3">test3</li>  
    </ul>  
  
d 选中这个标签以及标签内的文本。  
  
n 移到下一个标签。  
  
N 移到上一个标签。  
  
i 改变img标签  
    <img src="foo.png" >  
  
j 分割标签，或者合并标签  
<div class="foo"></div>  
<div class="foo"/>  
  
/ 注释标签  
  
c code pretty  
    <p>Writing in C language</p>  
      
    int main(){  
        puts('hello, world');  
    }  
  
