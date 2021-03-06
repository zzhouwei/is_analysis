# 基于GitHub的实验管理平台的分析与设计

### 成都大学信息科学与工程学院
|    学号  |   班级    |    姓名  |   照片     |
|:--------:|:--------: | :----------: | :-------:|
|201510414430|软件(本)15-4|周威 |![](./myself.jpg)|

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理学生实验的web系统，设计目的在于减轻全校教职工的实验批改负担以及方便学生提交实验，查看自己的成绩。老师发布的实验项目和学生提交的实验均显示在GitHub页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名和密码，二是提交实验，三是查看自己各课程实验的成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的实验并评分，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到对应学生的每个GitHUB课程的实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，并设置了多项评分细则，最低为0分。
- 系统自动计算每个学生每一科的所有实验的平均分。
    
## 2. 系统总体结构
![](xtztjg.JPG)
界面设计参见：https://zzhouwei.github.io/is_analysis/test6/ui/home.html
    
## 3. 用例图设计 [源码](./src/usercase.puml)
![](./yonglitu.png)

## 4. 类图设计 [源码](./src/leitu.puml)
![](./leitu2.png)

## 5. 数据库设计
### [参见数据库设计](数据库设计.md)

## 6. 用例及界面详细设计
### 说明，由于在用Axure设计界面时用的是动态面板，导致在导出网页时多个功能界面的路径都是一样的，如“学生查看成绩”，“学生上传实验”的路径都和“用户个人信息维护”的路径一样，上传后的地址都是“.../test6/ui/page_2.html”，烦请老师在批阅的时候手动点击界面上的按钮进行跳转，多有不便，见谅。
- ### [“用户个人信息维护”用例](./个人信息维护.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ### [“登录”用例](./登录.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/home.html)

- ### [“登出”用例](./登出.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ### [“学生查看个人成绩”用例](./查看个人成绩.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ### [“查看全班成绩”用例](./查看全班成绩.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ### [“学生上传实验”用例](./学生上传实验.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ###  [“学生选课”用例](./学生选课.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)

- ### [“查看课程”用例](./查看课程.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_2.html)


- ### [“老师发布实验”用例](./老师发布实验.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_1.html)
    

- ### [“老师评定成绩”用例](./老师评定成绩.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_1.html)
    
- ### [“老师选课”用例](./老师选课.md),[界面](https://zzhouwei.github.io/is_analysis/test6/ui/page_1.html)
   

