author: Martin
date: 2015-03-12 09:14:15
title: (一) C++开发者都应该使用的10个C++11特性 -- auto

在C++11之前, auto关键字用来指定存储期, 表明变量具有本地范围, 块范围的变量声明（如for循环体内的变量声明）默认为auto存储类型.
其实大多普通声明方式声明的变量都是 auto 变量, 他们不需要明确指定auto关键字, 默认就是auto的了, auto变量在离开作用域是会变程序自动释放.

在新标准中, auto 的功能变为**自动类型推导.
**auto 通知编译器去根据初始化代码推断所声明变量的真实类型.
各种作用域内声明变量都可以用到它, 如: 名空间中, 程序块中, 或是for循环的初始化语句中.
需要注意的是, auto不能用来声明函数的返回值.

    auto i = <span style="color: #800080">42</span>;        <span style="color: #008000">//</span><span style="color: #008000"> i is an int</span>
    auto l = 42LL;      <span style="color: #008000">//</span><span style="color: #008000"> l is an long long</span>
    auto p = <span style="color: #0000ff">new</span> foo(); <span style="color: #008000">//</span><span style="color: #008000"> p is a foo*</span>




在泛型编程中, auto 关键字的出现让一切变得很简单了.
 p 
