<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：addScore  [返回](../README.md)
用例： [评分](../用例/评分.md)

- 功能：
    对学生的实验打分

- 权限：
    老师：必须先登录。

- API请求地址：
    接口基本地址/v1/api/addScore

- 请求方式 ：
    POST

- 请求实例：

        {
            "studentId":"201510414117",
            "experimentId":"1239",
            "score":{
                "item":"ui界面",
                "value":"36"
            },
            "score":{
                "item":"复杂度",
                "value":"39.5"
            }
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |studentId|学生的id号，注意这不是学号|
  |experimentId|实验id|
  |item|评分项的名字|
  |value|该评分项的得分|

- 返回实例：

        {
            "status": true,
            "info": null,

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，