<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getOwnGrade  [返回](./README.md)
用例： [学生查看个人成绩](./查看个人成绩.md)

- 功能：
   返回某个学生某一课程的全部实验成绩
    
- 权限：
    学生：只能查看自己的成绩，即接口参数studentid必须等于登录学生的studentid
    
    
- API请求地址： 
    接口基本地址/v1/api/getOneStudentResults/<studentid>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |studentid|学生的学号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "studentid": "201510315203", 
            "github_username": "zzhouwei", 
            "class": "软件(本)15-4", 
            "name": "陈松华", 
            "avgresult":90.5,       
            "data": [
                {
                "test_id":1,
                "web_exists": true, 
                "result": 91, 
                "memo":"本实验做得好",
                "update_date": "2018-04-02 13:48:01"
                }, 
                {
                ...其他实验
                }
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |studentid|学号|
  |github_username|学生的gitHub用户名|
  |class|班级|
  |name|真实姓名|   
  |avgresult|实验平均成绩|   
  |data|所有实验的成绩和评语|
  |test_id|实验编号|
  |web_exists|本实验的GitHub网页是否存在|
  |result|本实验成绩，可以为空，为空表示没有批改，没有批改的实验不入平均成绩，为0分则要计入平均成绩，所以成绩为空和为0是不一样的。|
  |memo|本实验老师的评价，可以为空|
  |update_date|本实验老师的批改日期，可以为空|

