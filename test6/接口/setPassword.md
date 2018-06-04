﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setPassword  [返回](../README.md)
用例： [修改密码](../用例/修改密码.md)

- 功能：
    修改（设置）用户的密码。
    
- 权限：
    学生/老师：修改自己的密码，必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/setPassword

- 请求方式 ：
    POST

- 请求实例：

        {
            "username":1234,
            "password":AF#W@#AAAASDF
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |username|用户的ID号。对应表login.username的值|
  |password|用户的密码。| 
  
- 返回实例：

        {         
            "status": true,
            "info": null,    

        }
 
- 返回参数说明： 
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，