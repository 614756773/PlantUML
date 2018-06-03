﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：updateStudentInfo  [返回](../README.md)

- 功能：
    修改学生的信息。
    
- 权限：
    学生：修改自己的信息，必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/updateStudentInfo

- 请求方式 ：
    POST
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的ID号。对应表student.id的值|
  
- 请求实例：

        {         
            "ID":"123456",  
            "studentNumber":201510414117" 
            "name":"秦著",
            "github":"https://github.com/614756773/is_analysis",
            "sex":"男",
            "nation":"汉"           
        }
 
- 请求参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |ID|自然主键|
  |studentNumber|学号|
  |name|用户的真实姓名|  
  |github|gitHub地址|
  |sex|性别|
  
- 返回实例：

        {         
            "status": true,
            "info": null
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
