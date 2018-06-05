<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setGrade  [返回](./README.md)
用例： [老师评定成绩](./老师评定成绩.md)

- 权限：
    老师登录后才能批改评定
   

- 功能：
    为某一个同学的某一实验打分。

- API请求地址：
   接口基本地址/v1/api/setGrade(aGrade&bGrade&cGrade&dGrade&memo)


- 请求方式 ：
    GET

- 请求参数说明:
   
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |aGrade|创新得分|
  |bGrade|完成度得分|
  |cGrade|功能性得分|
  |dGrade|复杂度得分|
  |memo|老师的实验评价|
 


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

