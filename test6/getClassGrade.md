<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getClassGrade  [返回](./README.md)
用例： [查看全班成绩](./查看全班成绩.md)

- 权限：
    学生/老师：不能看到具体的每一评分项得分也不能看到评价，只能获得每一个实验的总分(全班成绩属于宏观不关心细节)
   

- 功能：
    返回某一个课程的全班实验成绩列表。

- API请求地址：
   接口基本地址/v1/api/getClassGrade

- 请求方式 ：
    GET

- 请求参数说明:
    无

- 返回实例：

        {
            "status": true,
            "info": null,
            "students": 60,
            "data": [
                {"student1": 
					{"name":周威，
					 "experiment1":85,
					 "experimnet2":90,
					 "experimnet3":88,
					 "experiment4":90,
					 "average":88.25
					}，
					"student2": 
					{"name":张三，
					 "experiment1":85,
					 "experimnet2":90,
					 "experimnet3":88,
					 "experiment4":90,
					 "average":88.25
					}，
					.....
					.....
				"student60":
				 {"  name":张三，
					 "experiment1":85,
					 "experimnet2":90,
					 "experimnet3":88,
					 "experiment4":90,
					 "average":88.25
					}，
				]
               
                "CLASS": "软件(本)15-4",
                "course": "数据机构与算法",
               
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |students|学生的数量|
  |data|所有学生成绩的数组|
  |studentn|具体某个学生的编号|
  |name|学生姓名|
  |experimentn|具体某一个实验的成绩|
  |average|某一个学生的全部实验的平均成绩|
  |CLASS|班级|
  |course|课程名|
