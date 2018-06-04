<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：studentLookCourse  [返回](../README.md)
用例： [学生查看课程](../用例/学生查看课程.md)

- 功能：
    学生查看自己选了哪些课程，并且能够查看任课老师的信息

- 权限：
    学生：必须先登录。

- API请求地址：
    接口基本地址/v1/api/studentLookCourse/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |student_id|学生id|

- 返回实例：

        {
            "course": {
                "id": "1240",
                "name": "信息系统",
                "credit": "3.5",
                "teacherName": "赵卫",
                "teacherId":"12345679"
            },
            "course": {
                "id": "1259",
                "name": "linux",
                "credit": "3.5",
                "teacherName": "王五",
                "teacherId":"12345610"
            }
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:-------------|
  |course|课程，是个嵌套json|
  |id|课程号|
  |name|课程名称|
  |credit|学分|
  |teacherName|老师名称|
  |teacherId|老师id|