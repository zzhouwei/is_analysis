<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setUpload  [返回](./README.md)
用例： [上传实验](./学生上传实验.md)

- 权限：
    学生：只有学生登录后才能上传
   

- 功能：
    学生提交实验作业到指定课程的指定实验目录下。

- API请求地址：
   接口基本地址/v1/api/setUpload

- 请求方式 ：
    GET

- 请求参数说明:
    无

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
 