<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setStudnetChoose  [返回](./README.md)
用例： [学生选课](./学生选课.md)

- 功能：
    将学生的选课记录记录到STUDENT表。
    
- 权限：
    学生登录。    
    
- API请求地址： 
    接口基本地址/v1/api/setStudentChoose(stuid&courseid)

- 请求方式 ：
    POST

- 请求实例：

        {
            "userid":"201510414430",
			"courseid":"6545498"
            
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |stuid|学生编号|
  |courseid|课程编号|

- 返回实例：

        { 
            "status": true,
            "info": null,
			
			
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|



