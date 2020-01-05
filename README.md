# 18Python课程期末作业
* 我们小组由17级[莫文俊](https://github.com/wenjunmo/DataStory_Interactive-Visualization/blob/master/README.md)，18级[刘瑜鹏](http://crayon3.pythonanywhere.com/)，[刘宇](https://github.com/wenjunmo/DataStory_Interactive-Visualization/blob/master/README.md)组成。我们的小组合作的web应用主题为**世界五百强公司折射的全球经济结构分析**，旨在分析世界500强企业中美经济结构的差异化现象，结合数据分析图表展示差异化因素，并在最小可行性推断未来新兴科技发展方向。    
  
* 我们的项目使用交互可视化工具Plotly/Pyecharts，搭建Flask框架实现可互动交互界面，并且呈现数据故事引导用户对数据进行思考。刘瑜鹏同学的部分进行了全球情况的展示，我的部分由刘瑜鹏同学的部分衍生出来，细化分析*世界500强公司折射的中美经济结构差异化现象*，展示更多详细数据与对比图。  

* [我的代码Github URL：**https://github.com/liuyu19/python_final**](https://github.com/liuyu19/python_final)
* [我的pythonanywhere URL/云服务器的域名提交 URL: **http://liuyu18.pythonanywhere.com/**](http://liuyu18.pythonanywhere.com/)  

## 项目描述:  
1.已达到基本要求
> 实现 交互功能 (Html表，至少做到表的交互没图假设下)√  
> 实现 **部署在 pythonanywhere 可用**√    
> 基本README.md技术文档总结项目说明√  
> * 自己提供数据，但数据量>250个√    
> * Html5界面设计包含CSS样式√  
> * 必须部署在 pythonanywhere 并可用√   
> * H5页面设计包含CSS样式√

HTML档描述：    
我们小组一共有三个HTML文档，example1.html是代码生成的柱状图，render.html负责页面图表的展示，我们增加了选择按钮和渐变背景，认真配置了css以符合表格的颜色，增加美观性，example2.html负责下拉框选择不同的选项。
    
PYTHON档描述：  
我们小组一共有两个py文档，jiaohu.py用来保证页面的跳转和交互功能。vsearch.py负责数据的可视化。  

webapp的动作描述：在顶部导航栏设置了按钮和超链接，可以跳转到不同的图表。下拉选择框和结论分开设置，便于观察。
2.数据传递描述: 
用render_template()方法传递表格和数据，def（）定义函数。
