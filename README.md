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
results2.html负责下拉框选择不同的选项，修改了css使背景颜色渐变，增加了<header>并且额外设置了字体的大小和格式使之居中，突出主题。定义下拉框的标签<select>我们运用了if函数来筛选数据，传递后生成表格与柱状图。
example1.html是代码生成的柱状图。
render.html负责页面图表（pyecharts）的展示与结论，我们增加了选择按钮和渐变背景，认真配置了css以符合表格的颜色，增加美观性。同时插入了box修改了边框形状（border-radius），使边框半径改变，从而呈现曲线。

    
PYTHON档描述：  
我们小组一共有两个py文档，jiaohu.py用来保证页面的跳转和交互功能，在这里我一定要强调一下我遇到的困难，也可以给各位同学一个建议，在我利用Python增删改查等方法筛选好中国和美国的数据之后，导入csv却意外的发现无法实现flask，缺少cufflinks模块，我尝试了市面上的所有方法，包括但不限于直接点击红色灯泡安装，利用环境变量安装，开cmd用命令行pip install cufflinks安装，最后尝试了朴素方法重装conda以及pycharm解决了这个问题。vsearch.py负责数据的可视化。 

WEBAPP的动作描述：  
在顶部导航栏设置了按钮和下拉框，点击“do it”按钮通过下拉框可以跳转到不同的页面（/hurun），图表能够有悬停阴影，注释等。  
另一个结论按钮会显示不同的图表，同样有悬停阴影与注释，还实现了地图和地区的联动。下拉选择框和结论分开设置，便于观察。  

2.数据传递描述: 
用render_template()方法传递表格和数据，def（）定义函数。
