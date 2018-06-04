<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：studentLookScore  [返回](../README.md)
用例： [学生查看成绩](../用例/学生查看成绩.md)

- 功能：
   学生查看自己的成绩
   可以按照学期，课程，实验来查看

- 权限：
    学生：必须先登录。

- API请求地址：
    接口基本地址/v1/api/studentLookScore/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |student_id|学生id|

- 返回实例：

        {
            "score": {
                "courseId",1234",
                "course": "信息系统",
                "experiment": "流程图的制作",
                "experimentId":"2014",
                "value": "81",
            },
            "score": {
                "courseId",1234",
                "course": "信息系统",
                "experiment": "活动图的制作",
                "experimentId":"2014",
                "value": "95",
            },
            "score": {
                "courseId",1024",
                "course": "linux",
                "experiment": "shell变成",
                "experimentId":"779",
                "value": "85",
            }
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:-------------|
  |score|成绩，是个嵌套json|
  |courseId|课程号|
  |course|课程名称|
  |experiment|实验名称|
  |value|当前实验的平均成绩|