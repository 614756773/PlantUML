<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：teacherLookCourse  [返回](../README.md)
用例： [老师查看课程](../用例/老师查看课程.md)

- 功能：
    教师查看自己已选的课程,并且能够查看哪些学生选了自己的课

- 权限：
    老师：必须先登录。

- API请求地址：
    接口基本地址/v1/api/teacherLookCourse/<teacher_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |teacher_id|老师id|

- 返回实例：

        {
            "course": {
                "id": "1240",
                "name": "信息系统",
                "credit": "3.5",
                "stuNum": "60"
            },
            "course": {
                "id": "1259",
                "name": "linux",
                "credit": "3.5",
                "stuNum": "45"
            }
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:-------------|
  |course|课程，是个嵌套json|
  |id|课程号|
  |name|课程名称|
  |credit|学分|
  |stuNum|当前课程下的学生人数|