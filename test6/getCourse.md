<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getCourse  [返回](./README.md)
用例： [查看课程](./查看课程.md)

- 功能：
    获取已经选择的课程。
    
- 权限：
    学生，老师。    
    
- API请求地址： 
    接口基本地址/v1/api/getCourse(USERID)

- 请求方式 ：
    POST

- 请求实例：

        {
            "userid":"201510414430",
            
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |userid|学生学号或者老师的工号|

- 返回实例：

        { 
            "status": true,
            "info": null,
			{    
			 "courseNumber"：5
			"course1":数据结构与算法,
			"course2":C语言,
			......
			"course5":大学英语
			}
			
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |courseNumber|课程数量|
  |coursen|具体一个课程名，n代表数字取值在1-courseNumber|


