

## **IDetailTracker.SaveChanges(bool batchExecute = false) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Updates the database by executing the data changes tracked by a ModelMapper instance.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  IDbResult SaveChanges(bool batchExecute = false);
```

**Parameters**

`batchExecute`	System.Boolean

当存在多条待执行的SQL DML时，是批量执行还是一条一条执行。

Whether to execute the SQL DML one by one or in a batch, when there are more than one SQL DML to be executed.

默认为false，表示一条一条执行。

The default value is false which indicates SQL DML will be executed one by one.

当需要执行的SQL DML较多时，建议设置为true，可减少数据库请求次数提供执行效率。

When there are a large amount of SQL DML, it is recommended to set to true, to reduce the database requests and improve the execution speed.

**Returns**

[Appeon.CoreService.Data.IDbResult](../../IDbResult/IDbResult.html)

返回一个接口，可以利用该接口的各种属性方便地获取在数据库执行后得到的结果。

Returns an interface whose property can be used to conveniently get the result of the executed database operation.

### **Remarks**

It has the same effect as calling the IModelMapper.SaveChanges method. See IModelMapper.SaveChanges for more info.

### **Examples**



### **Applies to**

.NET Standard 

2.x