﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getUserInfo  [返回](../README.md)

- 功能：
    查看用户的所有信息。
    
- 权限：
    学生/老师：查看自己的信息，必须先登录，不能查看其他用户的信息。    
    
- API请求地址： 
    接口基本地址/v1/api/getUserInfo/<student_id>

- 请求方式 ：
    GET
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的ID号。对应表student.id的值|
  
- 返回实例：

        {         
            "status": true,
            "info": null,
            "ID":"123456",  
            "studentNumber":201510414117" 
            "name":"秦著",
            "github":"https://github.com/614756773/is_analysis",
            "sex":"男",
            "nation":"汉"
            "type":"学生"            
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |ID|学号或者工号|
  |name|用户的真实姓名|  
  |github|gitHub地址|
  |type|用户类型：老师或者学生|
  |sex|性别|
  |nation|民族|

