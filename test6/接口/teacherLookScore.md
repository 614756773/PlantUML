<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：teacherLookScore  [返回](../README.md)
用例： [老师查看成绩](../用例/老师查看成绩.md)

- 功能：
   老师查看自己教学课程下的所有学生成绩
   可以按照学期，课程来进行选择，查看成绩时默认显示
   学生的所有实验的平均成绩，点击可以查看详细情况

- 权限：
    老师：必须先登录。

- API请求地址：
    接口基本地址/v1/api/teacherLookScore/<teacher_id>/<term_id>/<course_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |teacher_id|老师id|
  |term_id|学期id|
  |course_id|课程id|

- 返回实例：

        {
            "row": {
                "studentNumber",201510414117",
                "name": "秦著",
                "avgScore": "83.3"
            },
            "row": {
                "studentNumber",201510414110",
                "name": "小白",
                "avgScore": "81.5"
            }
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:-------------|
  |studentNumber|学号|
  |name|学生姓名|
  |avgScore|当前课程的所有实验的平均成绩|