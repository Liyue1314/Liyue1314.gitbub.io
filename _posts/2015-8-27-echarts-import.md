---
layout: post
title: 模块化单文件引入ECharts步骤
category : echarts
tagline: "示例笔记本"
tags : [演示,echarts]
---
{% include JB/setup %}

##模块化单文件引入ECharts

    1.为ECharts准备一个具备大小（宽高）的Dom（当然可以是动态生成的）
    2.通过script标签引入echarts主文件
    3.为模块加载器配置echarts的路径，从当前页面链接到echarts.js所在目录，见上述说明
    4.动态加载echarts及所需图表然后在回调函数中开始使用（容我罗嗦一句，当你确保同一页面已经加载过echarts，再使用时直接require('echarts').init(dom)就行）

详见[入门教程（ Getting started）>>](http://echarts.baidu.com/doc/start.html)

{% highlight java linenos %}
public class HelloWorld {
    public static void main(String args[]) {
      System.out.println("Hello World!");
    }
}
{% endhighlight %}

```` java
public class HelloWorld {
    public static void main(String args[]) {
      System.out.println("Hello World!");
    }
}
````