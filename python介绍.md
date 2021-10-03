# python介绍

​		Hello大家好，我是浮磊，大家也可以叫我Eric。这篇内容我们来探讨一下关于python的三个问题。他们分别是：python是什么？它可以用来做什么？为什么它如此受欢迎？

## python是什么？它可以做什么？

​		python是当前世界上发展最快、最受欢迎的编程语言，除了专业的软件工程师，还有其他很多职业的人员在使用python，比如数学家、数据分析师、科学家、会计、网络工程师甚至是小朋友！因为它是一种非常适合初学者的编程语言。因此各行各业的人都在用python解决各种问题，例如可视化数据分析、人工智能、机器学习、自动化，实际上这也是非软件工作人员使用python的主要用途之一。如果你也经常需要处理重复性的工作任务，例如每天都要将自己的图片或视频上传到网上，你就可以编写一个python脚本来自动帮我们实现上传的操作，帮你节省时间。再者如果你需要处理很多的excel表格、pdf、从网上下载各种资源你都可以使用python自动执行所有这些工作。所以不论你从事任何行业，都可以使用python让你的工作变的更轻松。你可以使用python来构建网站、手机或电脑桌面程序、软件测试甚至是黑客攻击。所有python是一种多用途的易学习的编程语言。

## python为什么如此受欢迎？

​		如何你有一定的编程经验，你可能会说“这些工作我都可以使用其他的编程语言来完成，python有什么大不了的呢？”使用python，你可以使用更少的代码在更短的时间内解决复杂的问题。

​		我们来看一个例子，假设我们要提取一段文字中的数字内容，这是C#编写的代码：

```c#
using System;
using System.Text.RegularExpressions;
public class HelloWorld{
       static void Main(string[] args){
			string str = "提取123.11abc提取"; 
			str=Regex.Replace(str, @"[^\d.\d]", "");
			if (Regex.IsMatch(str, @"^[+-]?\d*[.]?\d*$"))
			{
				decimal result = decimal.Parse(str);
				Console.WriteLine("使用正则表达式提取数字");
				Console.WriteLine(result);
			}
        }
 }
```

这是使用Java编写的代码

```java
public class HelloWorld {
    public static void main(String[] args) {
		String str = "提取123.11abc提取";
		str=str.trim();
		String str2="";
		if(str != null && !"".equals(str)){
			for(int i=0;i<str.length();i++){
				if(str.charAt(i)>=48 && 		                     str.charAt(i)<=57){
				str2+=str.charAt(i);
				}
			}
		}
		System.out.println(str2);
	}
}
```

这是python编写的代码

```python
import re
ss = '提取123.11abc提取'
s = re.findall("\d+.\d+",ss)[0]
print(s)
```

可以看到这门语言是多么的简洁和干净，这还是个开始，python使用简单的语法让很多繁琐的事情变得非常容易。并且python作为一种高级语言，你不必像在C++中那样担心内存管理这样复杂的问题。它还是跨平台的，你可以在windows,mac,linux上创建和运行python程序。python已经存在20多年了，拥有庞大的社区，你可以在其中得到非常有用的帮助，它拥有丰富的工具、库、框架，这意味着当你想要实现某些功能时，其他人以前已经做过。

## 总结

所以简而言之，python是一种具有简单、干净对初学者友好语法的多用途语言。从技术上讲，python能实现的功能，你都可以用其他编程语言实现，但python的简单和优雅使它比其他语言更受欢迎。因此，无论你是程序员还是零基础的初学者，学习python都会为你创造更多的机会。如果你觉得这篇文章对你有帮助，请点赞，帮忙分享给朋友，写作不易，谢谢你的支持。

