# Java Bug记录

```1.SpringBoot整合 Mybatis```
	  
mapper.xml文件位置无误，mapper接口方法调用无误，返回如下错误：
## org.apache.ibatis.binding.BindingException: Invalid bound statement (not found): （mapper路径+方法名）
    
原因：mapper.xml 开头 namespace 路径错误，应写mapper接口的全路径名
