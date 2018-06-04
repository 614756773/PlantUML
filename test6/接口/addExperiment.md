﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：addExperiment  [返回](../README.md)

- 功能：
    新添加实验。

- 权限：
    老师:只能对自己已选课程添加实验

- API请求地址：
    接口基本地址/v1/api/addExperiment

- 请求方式 ：
    POST

- 请求实例：

        {
            "name":"流程图绘制",
            "desc":"流程图应该这样做：blablablasblabl...",
            "courseId":"20161",
            "scoreitem":{
                "sidesc":"UI界面",
                "value":"40",
            },
            "scoreitem":{
                "sidesc":"复杂度",
                "value":"60",
            }
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |name|实验名|
  |desc|对实验的描述|
  |courseId|课程号|
  |sidesc|评分项的名字|
  |value|分值|

- 返回实例：

        {
            "status": true,
            "info": null,

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，

