<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：stuLookExperiment  [返回](../README.md)
用例： [查看老师布置的实验](../用例/查看老师布置的实验.md)

- 功能：
    学生查看所选课程的实验要求，可以查看到所属课程，发布时间等

- 权限：
    学生：必须先登录。

- API请求地址：
    接口基本地址/v1/api/stuLookExperiment/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |student_id|学生id|

- 返回实例：

        {
            "row": {
                "courseName": "linux",
                "experimentName": "shell编程",
                "experimentId":"12134",
                "github": "https://github.com/zwdbox/is_analysis/blob/master/test1.md",
                "time": "2018-06-04"
            },
            "row": {
                "courseName": "linux",
                "experimentName": "shell编程2",
                "experimentId":"12135",
                "github": "https://github.com/zwdbox/is_analysis/blob/master/test1.md",
                "time": "2018-06-05"
            }
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:-------------|
  |courseName|课程名称|
  |experimentName|实验名称|
  |experimentId|实验id|
  |github|该实验的github地址|
  |time|发布时间|