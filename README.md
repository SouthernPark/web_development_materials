# web_development_materials

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)


## Table of Contents
- [任务](#任务)
- [工具](#工具)
- [后端学习资料](#后端学习资料)
- [前端学习资料](#前端学习资料)
- [会议记录](#会议记录)
	- [1st_meeting](#1st_meeting)
	- [2nd_meeting](#2nd_meeting)
	- [3rd_meeting](#2nd_meeting)
- [受众](#受众)
- [画图](#画图)
- [需求](#需求)
- [功能](#功能)
- [提议](#提议)

## 任务  

>DDL 2020年2月14日

>第二次会议 任务分配：   
两人一组 调换任务 检查补充     
Alen Betty：背景 风险规划 整合文档 受众 调查问卷 分析 文献   
强强 栋栋：画图：各种图 use case ; boundary; data-flow; ER 图   
托比 倍倍：文字描述：用户需求 功能与非功能需求 系统描述 事务需求  

## 工具  

>后端:  
Python & Flask & SQL  

>前端:   
Css & javascript & html  

>手机APP:   
Android studio ?     
纯网站开发/混合开发   





## 后端学习资料
>Sherlock的学习资料:

		flask 快速入门教程 : https://www.youtube.com/watch?v=RWviEK1Si68&list=PLDFBYdF-BxV1G4FBpG1EMyFtbsbZuJOvD

>Bruce的学习资料:

		none


## 前端学习资料

>Toby的学习资料:

		谷歌地图API: https://www.runoob.com/googleapi/google-maps-api-key.html
		JavaScript教程: https://www.w3school.com.cn/js/index.asp
		CSS教程: https://www.w3school.com.cn/css/index.asp
		HTML教程: https://www.w3school.com.cn/html/html_layout.asp

>Park的学习资料:
		
		HTML CSS教程: https://www.bilibili.com/video/av52670599?from=search&seid=13457783868944189566

>Betty的学习资料:
		
		IBM垃圾分类API : https://github.com/IBM/watson-waste-sorter

>Alen的学习资料:
		
		none


## 会议记录



### 1st_meeting

>Documented by Toby  
第一次会议记录在上方的 1st meeting record.docx 文件中  

### 2nd_meeting

>Documented by Betty  
第二次会议记录记录在上方的2nd meeting.docx文件里   
 

>下次开会  
先准备开始requirement 文档 下次开会交 再调换部分    

### 3rd_meeting

>开会准备:  
 第二次会议，我们选出了系统的受众(User). 第三次会议，我们将确定系统的User.
 


## 受众  
>1.上门收垃圾(用户):  
House个人垃圾：一周收一次 临时收垃圾  
公寓(Apartment)负责人：花钱临时收垃圾  
大型垃圾处理站  

>2.垃圾处理公司:  
垃圾运给处理公司 利用         
意义： 盈利 环保  

## 画图 
>用例图：需求描述  
时序图  
活动图  

## 需求   
User requirements:  
Customer:

	1.Customer shall sing up and log in before using this application  
	2.Customer can pay a fee to apply for additional garbage collection times  
	3.Customer can purchase long - term services  
	4.Customer can choose to stick with the service or give up the service based on the quotation provided by the manager  
	5.Customer can apply to cancel the order  
Driver:  

	1.Driver can log in directly from their work account  
	2.Driver can view the path plan  
	3.Driver can update the status of the application  

Manager： 

	1.Managers can log in directory from their work account  
	2.Manager can view the user’s application and send the quote  
	3.Manager can approve the customer’s request for cancellation  
	4.Manager can delay or cancel the service  


## 功能   
>路径规划  
简单垃圾分类：拍照 或者输文字 有无API？  
按什么分类  
垃圾桶位置  

>垃圾车时间划分  
1.定时定点（7天）  
2.预约 分段考虑时间点（有记录 没到七天不用去）  
3.优先级 多少户才可以走 收费 实时价格  

## 提议
>情景引入:  
Trash公司是Liverpool的一家垃圾管理公司，主要进行大型的垃圾回收(公寓垃圾回收，学校垃圾回收，个人house垃圾回收等)。Trash公司要求我们建立一个帮助公司处理业务的系统.  
Trash公司希望, 新用户通过 网站(或者手机APP) 提交申请。公司经理看到申请后，撰写初期合同，与用户约定时间商议，签署最终合同。  
合同签署后，公司经理将该用户的公寓加入垃圾管理计划。  
为了方便公司司机回收垃圾，Trash公司希望我们设计一个给司机分配任务，帮助司机规划路线的功能。  
Trash公司发现，很多回收的垃圾没有被正确的分类。导致这一问题的原因之一是，用户对垃圾如何分类没有正确的认识。因此，Trash公司希望提供给用户垃圾分类的功能。  

>Sherlock's  proposal:  
我们设计的系统有两个子系统组成: 用户系统 和 员工系统。用户系统应该与员工系统相互独立。    
>1.用户系统  
用户系统为用户(User)设计。该系统通过网站(如:www.user.com)的形式暴露给用户。用户通过该系统后能做的task有:  

		(a)注册
		(b)找回密码
		(c)登录  
		登录后的功能有  
		(d)申请Trash公司的垃圾管理服务[填写联系方式，公寓地址] [申请后等待Trash公司经理的约谈]  
		(f)向Trash公司发送 收垃圾 请求 (只有当签完合同后才有这个页面)
		(g)垃圾分类
		(h)附近的垃圾公共站点查询[我觉得这个有点很Trahs公司的目的不相符]
		
		
		用户系统的数据库schema:  
		User(username, password, email)  
		Constrains：   
		username 和 email必须唯一。Primary Key (用户的账号名不能重复，用户的邮箱不能重复)

>2.员工系统  
员工系统为 经理(Manager) 和 司机(Driver)设计。该系统通过网站(如:www.staff.com)暴露给员工。员工通过该系统能够做:  
		
		Manager:
		(a)登录
		(b)忘记密码
		登录成功后
		(c)查看是否有用户申请垃圾管理服务。 
		[如果有 Manager应该撰写初期合同， 与用户约谈，签订合同]     
		[谈话过程中，用户需要提供自己的垃圾场地址，以及自己需要多长时间的服务].    
		
		(d)根据合同向Service数据库中输入信息。  
		
		Driver:  
		(a)登录
		(b)忘记密码后
		登录成功后:
		(c)查看自己的任务  [路径规划]
		(d)每清理完一会，点击Finished

		员工系统的数据库schema:
		Manager(StaffID, name, telephine, email)   
		Driver(StaffID, name, telephone, email)   
		Service(ServiceID, username, wasteyard_address, lastTimeClean, require?, timeDDL)   
		Service数据库解释:  
		ServiceID: Primary Key 唯一性  
		username: 用户账号的名字. Foreign Key from User database. 可以重复(一个用户可能有多个house需要提供服务)  
		wasteyard_address: 用户的垃圾场地址。  
		lastTimeClean:上一次清理的事件  
		require?: 用户是否请求清理  
		timeDDL:我们的服务截止日期。
		
		
		

## License

[MIT](LICENSE) © Richard Littauer
