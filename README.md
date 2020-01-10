# 智能博物馆产品需求文档

| 发布日期   | 2019-12-10     |
| ---------- | -------------- |
| 项目名称   | 智能博物馆 |
| 项目现状   | 完成        |
| 项目所有者 | 李铮         |
| 项目设计师 | 李铮         |
| 项目开发者 | 李铮         |
| 项目测试者 | 李铮         |

# 智能博物馆产品需求文档

## Part1.一句话价值主张
- 针对两种类型人群开发一款动静结合的智能语音导览的APP，并适用于大众群体
## Part2.一分钟价值主张  
### 价值宣言
- 为用户提供
### 产品目标：用户可以通过语音导览享受到在线语音交互。  
### 用户痛点：
1. 用户到达博物馆后，想找的展品位置在哪。
2. 当用户到达展品处后，想了解展品的简介。
3. 当博物馆发生突发事件时，展馆可以第一时间就近调动相关的安保人员进行维护处理。
4. 博物馆想要知道哪些展品比较受欢迎？展品摆放区域是否合理？
### 参观者（游客）用户需求分析：
1. 用户对智能语音导览的识别准确度    
通过线上调查和用户访谈等各种方式可知，用户对智能语音导览的准确度仍有一些建议，语音导览对场景的识别不够精确，需要在一定的范围内才能很好地识别场景。
2. 用户对智能语音导览的语音合成功能的需求     
针对博物馆的文物众多、分类细致的特点，用户所期待的是可以通过语音输入指定的相关类型文物检索来自助导览，并可以获得相关内容的介绍，可以通过前期获取博物馆文物的数据统计和资料收集，然后使用阿里巴巴的API的接口来实现用户输入语音，合成文字后转给导览器进行识别并反馈信息。  
3. 用户对智能语音导览器的人机交互需求    
随着语音助手的逐渐流行，人们更注重人机交互的功能实现，绝大部分的用户对于语音交互在导览器上实现十分期待，我们根据调查发现，各年龄层的用户在使用导览器时存在各种常见的问题，而这些常见的问题我们可以通过智能语音识别ASR、语音合成服务TTS、自然语音处理NLU三种技术的结合来实现导览器“能听”"会说"“智能问答和意图识别”等功能于一体，使得导览器具备理解用户和反馈信息的能力。

### 管理者（工作人员）需求分析：
1.管理者对于设备（导览器）的管理和调试功能的操作是否简便  
综合用户的需求，工作人员在派发导览器的时候，需向用户简单的介绍设备，并在给设备前确认设备可正常使用。 
2.工作人员对于导览器的更新是否会操作  
文物的收录和转移都需要人工对设备进行实时的更新，工作人员能否简易地使用导览器的后台来进行数据的修改，值得思考。  

![输入图片说明](https://images.gitee.com/uploads/images/2019/1113/075313_e57bd2b6_1831543.png "微信图片_20191112211607.png")
 
## 产品功能使用场景分析
### 对象1：用户： 
（1）用户到达博物馆后，不清楚自己想找的展品位置在哪，这时可通过产品对展品进行搜索，产品在屏幕上显示出相对应的位置以及可以通过配套耳机进行语音导览使用户能迅速到达。  
（2）当用户到达展品处后，对展品的简介无法理解时，可使用产品进行自定义语音导览

### 对象2：博物馆：
（1）当博物馆发生突发事件时，展馆可以第一时间就近调动相关的安保人员进行维护处理。因为语音导览器可以实时查看安保人员所处的位置。   
（2）博物馆想要知道哪些展品比较受欢迎？展品摆放区域是否合理？则可以通过语音导览器在后台系统对用户进行实时监测所得出来的数据，比如每日游客数量、游览行为数据，来对展品分布和游客接待工作进行调整。

## 使用到的API&数据库技术分析(所需API)
- 语音识别服务ASR ：将语音转换成文字的能力快速集成，打造出“能听”的应用。
- 语音合成服务TTS ：将文字转换为声音的能力快速集成，打造出“会说”的应用。
- 自然语音处理NLU ：集语义解析、智能问答、意图识别等功能于一体，让应用具备理解能力。

## 原型设计
![登录注册用户协议页](http://chuantu.xyz/t6/709/1577633303x989499252.jpg)
![找回密码](http://chuantu.xyz/t6/709/1577633240x989499252.jpg)
![未登录首页](http://chuantu.xyz/t6/709/1577633424x989559068.png)
![个人中心](http://chuantu.xyz/t6/709/1577633530x989559068.png)
![活动页 ](http://chuantu.xyz/t6/709/1577634038x989559068.jpg)


## 人工智能概率
- 语音合成服务TTS对于部分口音转译存在着部分无法合成的语音。
- 语音识别服务ASR在声音嘈杂的情况下可能无法精确识别语音内容。
- 自然语音处理NLU在在声音嘈杂的情况下可能无法精确识别语音内容。
