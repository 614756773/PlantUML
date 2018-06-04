<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：lookStuExperiment  [返回](../README.md)

- 功能：
    查看学生完成的实验

- 权限：
    老师

- API请求地址：
    接口基本地址/v1/api/lookStuExperiment/<student_id>/<experiment_id>

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |student_id|学生的ID号。对应表student.id的值|
  |experiment_id|实验id|

- 返回实例：

        {
            "github":"https://github.com/614756773/is_analysis/test3"
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |github|该学生做的实验的github地址|

