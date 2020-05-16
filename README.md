# 毕业设计 --基于B/S架构的JavaWeb在线考试系统



本文档只是对本人毕业设计的说明文档，并没有上传相关的源代码和数据库文件，如有需要，请联系作者。
邮箱：13834697883@163.com  QQ：2274747912  备注请写明您的意图！



### 项目亮点：
***
1. 前后端分离。
1. 用户登录权限区分和控制。
1. 防止横向越权和纵向越权。
1. 密码MD5明文加密。
1. 设计高复用的服务器响应对象。
1. guava缓存。
1. pojo，vo抽象模型。
1. 数据绑定对象。
1. Mybatis分页
1. Bootstrap。
1. artTemplate，artDialog，iframe前端模板使用。
1. select2、toastr、sweetalert等等前端插件的使用。
1. redis缓存。
1. 全局异常处理，拦截器权限统一检验。
1. echarts可视化技术对于学生成绩的统计（包括最高分，最低分，平均分，优秀率，及格率，不及格率的统计）
### 启动说明


***
项目为maven管理，集成了redis，所以在运行项目是先要下载redis并启动客户端，方可正常运行项目，由于只需要下载redis，无需其他配置，这里就不做过多说明。

### 最近更新
***
集成redis来保存用户登录信息，添加过滤器重置用户登录有效期。拦截器实现统一登录和权限校验。


### 项目采用前后端分离技术实现
***
- 框架：SSM（Spring，SpringMVC，Mybatis）
- 缓存：redis
- 数据库：MySQL
- IDE：Intellij IDEA
- 其他：Maven，Git， Tomcat， BootStrap， PageHelper， Echarts

### 项目实际效果
登录首页：不同用户角色的登录，进入相应的界面
![登录首页](https://upload-images.jianshu.io/upload_images/3256507-9a57fec3858718cb.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
---
教师成功登录界面查看题库信息
![教师成功登录界面查看题库信息](https://upload-images.jianshu.io/upload_images/3256507-fbf233d991419d88.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
忘记密码的回答问题功能
![忘记密码的回答问题功能.jpg](https://upload-images.jianshu.io/upload_images/3256507-b402058183a77fa3.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
忘记密码的重置密码功能
![忘记密码的重置密码功能](https://upload-images.jianshu.io/upload_images/3256507-5475f5a62fde0b3a.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
查看试卷界面
![查看试卷界面](https://upload-images.jianshu.io/upload_images/3256507-557ce686a0092098.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
查看所有试卷界面
![查看所有试卷界面](https://upload-images.jianshu.io/upload_images/3256507-6442c8bb751ee373.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
查看试题详情
![查看试题详情](https://upload-images.jianshu.io/upload_images/3256507-ae912dafbb5cdd6c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
查看试题详情界面
![查看试题详情界面](https://upload-images.jianshu.io/upload_images/3256507-887f3a99b5fbf3dc.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
新增试题界面
![新增试题界面](https://upload-images.jianshu.io/upload_images/3256507-d95b7d1a311e8e28.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
教师手动组卷
![教师手动组卷](https://upload-images.jianshu.io/upload_images/3256507-9d113a50cfc2394e.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
教师自动出题
![教师自动出题](https://upload-images.jianshu.io/upload_images/3256507-b56286e9bf47c9fb.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
查看参加考试学生成绩
![查看参加考试学生成绩](https://upload-images.jianshu.io/upload_images/3256507-8d9b3bc4e4387ee8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
管理试题功能
![管理试题功能](https://upload-images.jianshu.io/upload_images/3256507-b35b6834812a87c2.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
试卷预览界面
![试卷预览界面](https://upload-images.jianshu.io/upload_images/3256507-801f980aa0602cb3.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
试卷发布
![试卷发布](https://upload-images.jianshu.io/upload_images/3256507-e7e0565db904d5c1.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
试题数量统计界面
![试题数量统计界面](https://upload-images.jianshu.io/upload_images/3256507-de3de5e81c86f3bb.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


---
选择试卷发布的专业
![选择试卷发布的专业](https://upload-images.jianshu.io/upload_images/3256507-a2ed0b6b2da17107.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
分数区间饼状图统计
![分数区间饼状图统计](https://upload-images.jianshu.io/upload_images/3256507-7b8a3902f02f5ea8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
成绩区间统计
![成绩区间统计](https://upload-images.jianshu.io/upload_images/3256507-b46f69033fadc760.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
成绩区间统计饼图
![成绩区间统计饼图](https://upload-images.jianshu.io/upload_images/3256507-addae98b311532a9.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
成绩极值均值统计
![成绩极值均值统计](https://upload-images.jianshu.io/upload_images/3256507-926bd57c3b6291e3.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
成绩优秀率统计
![成绩优秀率统计](https://upload-images.jianshu.io/upload_images/3256507-2a25fdf56ffcfe69.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
学生成功登录界面
![学生成功登陆界面](https://upload-images.jianshu.io/upload_images/3256507-005fa6cfa652d466.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
学生查看试卷功能
![学生查看试卷功能](https://upload-images.jianshu.io/upload_images/3256507-f34b246a8ce96982.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
---
学生参加考试功能
![学生参加考试功能.jpg](https://upload-images.jianshu.io/upload_images/3256507-7310f17e4a6f2011.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
学生查看考试成绩柱状图展示
![学生查看考试成绩柱状图展示](https://upload-images.jianshu.io/upload_images/3256507-5c585961c6adc4c8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
学生查询成绩功能
![学生查询成绩功能](https://upload-images.jianshu.io/upload_images/3256507-4dfde984c32cba29.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
做了一个词云
![做了一个词云](https://upload-images.jianshu.io/upload_images/3256507-2bfb89cdf749d506.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
管理员通知管理
![管理员通知管理](https://upload-images.jianshu.io/upload_images/3256507-c6cf836bacfb23e2.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
管理员教师和学生管理
![管理员教师和学生管理](https://upload-images.jianshu.io/upload_images/3256507-767a2c0d75e12759.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
管理员对专业的管理
![管理员对专业的管理](https://upload-images.jianshu.io/upload_images/3256507-91f3cb5f9dfaacd1.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
年级统计可视化
![专业统计可视化](https://upload-images.jianshu.io/upload_images/3256507-14775a2cb1292a66.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
专业统计可视化
![专业统计可视化](https://upload-images.jianshu.io/upload_images/3256507-0f7d6712af2e7670.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
数据库截图
![数据库截图](https://upload-images.jianshu.io/upload_images/3256507-40f76c5a5d1cbf0d.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
代码截图
![代码截图](https://upload-images.jianshu.io/upload_images/3256507-a1025958c467c029.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
总体设计1
![总体设计1](https://upload-images.jianshu.io/upload_images/3256507-e2c80d9d856b670a.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
总体设计2
![总体设计2](https://upload-images.jianshu.io/upload_images/3256507-ccfaa9d02116804a.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
总体设计图
![系统总体设计](https://upload-images.jianshu.io/upload_images/3256507-adb45719d9b2dfd5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 系统功能
***
本系统的目标是实现智能化考试，教师可以进行管理试题，管理试卷，发布试卷，成绩统计可视化等操作。其中出题方式有两种，自动出题和手动出题。学生在参加完考试之后，系统会自动进行阅卷，并给出学生的考试成绩。学生可以实时看到自己的成绩，成绩可通过可视化图表进行展示。

### 系统的总体设计
***
**管理员用户**

管理员能够对通知，学生和老师的信息进行管理，拥有增加，修改，删除，查询通知信息，学生信息，老师信息的权限

**学生用户**

学生是参加考试的主体，学生参加完考试之后，可以查看到自己的成绩，同时，这些成绩也会以柱状图形式进行展示。

**教师用户**

教师能够对试题信息，试卷信息进行管理，教师能够以手动组卷和自动组卷两种方式进行组卷，教师能够发布组好的试卷，同时，教师能够查看学生的考试成绩，能够对学生的成绩信息进行统计，能够统计成绩的区间分布, 优秀率，及格率，最高分，最低分，平均分等信息，能够通过多种图表的方式进行可视化展示。

### 系统子模块介绍
***
（1）登录模块：为了实现系统的安全性，所有用户的密码都通过MD5加盐技术进行加密，即使数据库泄露也不能将密码破解
（2）重置密码模块：用户若忘记密码可以通过回答设置的问题和答案进行修改密码。
（3）通知管理模块：不同角色的用户登录系统后都可以查看到系统中所发的通知。
（4）试题管理：教师能够向试题库中新增试题，教师能够查看自己设置的试题。
（5）试卷管理：教师能够向试卷库中新增试卷，教师能够查看自己设置的试卷。
（6）出题管理：教师能够进行手工组卷和自动组卷，手工组卷需要教师手动操作，自动组卷可以按照条件自动设置试卷。
（7）成绩统计：实现了考生成绩的可视化展示，综合运用了柱状图，饼图等图表进行可视化展示，能够分析学生成绩的区间分布，优良率，及格率，最高分，最低分，平均分等信息，可以实时对学生成绩进行统计。帮助教师更好的分析学生的考试情况。

### 具体实现
***
前端HTML，CCS，JavaScript作为核心组件，使用BootStrap前端开发框架，使用jQuery作为JavaScript库，使用AJAX与服务端进行数据交互，使用Echarts进行可视化展示，使用SweetAlert 弹窗插件与用户进行交互，使用artTemplate模板引擎进行数据遍历与展示。

后端采用Spring框架进行整合，SpringMVC作为Web MVC框架,  使用Mybatis作为持久层框架，使用MySQL作为持久化数据库，使用Redis作为缓存数据库，使用Mybatis PageHelper作为分页技术，使用logback作为日志框架，使用Apache dbcp数据库连接池，使用Mybatis-generator进行自动生成Mapper，使用Maven进行项目依赖管理。

---
**本文档只是对本人毕业设计的说明文档，并没有上传相关的源代码和数据库文件，如有需要，请联系作者：邮箱：13834697883@163.com                 QQ：2274747912  备注请写明您的意图！**

        
      
