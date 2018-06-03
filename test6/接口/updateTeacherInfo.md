﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：updateTeacherInfo  [返回](../README.md)

- 功能：
    修改老师的信息。
    
- 权限：
    老师：修改自己的信息，必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/updateTeacherInfo

- 请求方式 ：
    POST
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |teacher_id|老师的ID号。对应表teacher.id的值|
  
- 请求实例：

        {         
            "ID":"1234",  
            "teacherNumber":12345679" 
            "name":"赵卫",
            "github":"https://github.com/zwdbox/is_analysis",
            "sex":"男",
            "title":"教授"           
        }
 
- 请求参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |ID|自然主键|
  |Number|工号|
  |name|用户的真实姓名|  
  |github|gitHub地址|
  |sex|性别|
  |title|职称|
  
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
