<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：teacherSelectCourse  [返回](../README.md)
用例： [教师选课](../用例/教师选课.md)

- 功能：
    教师选择要上的课程
    
- 权限：
    老师：必须先登录。    
    
- API请求地址： 
    接口基本地址/v1/api/teacherSelectCourse

- 请求方式 ：
    POST

- 请求实例：

        {
            "teacher_id":"12345679"
            "course_id":"1002,1035,2006"
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |teacher_id|老师id|
  |course_id|课程号|
  
- 返回实例：

        {         
            "status": true,
            "info": null,    

        }
 
- 返回参数说明： 
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，