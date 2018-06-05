<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setExperiment  [返回](./README.md)
用例： [发布实验](./老师发布实验.md)

- 权限：
    老师登录后才能发布实验
   

- 功能：
    将老师的实验发布到平台。

- API请求地址：
   接口基本地址/v1/api/setExperiment(experimentaim&experimentprocess&date&teacherid)

- 请求方式 ：
    GET

- 请求参数说明:
    |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |experimentaim|实验目的|
  |experimentprocess|实验过程|
  |date|最迟提交日期|
  |teacherid|老师编号|


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
