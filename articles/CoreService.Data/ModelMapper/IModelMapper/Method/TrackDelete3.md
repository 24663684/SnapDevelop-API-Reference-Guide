

## **IModelMapper.TrackDelete(ISqlDeleteBuilder deleteBuilder, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表的删除的操作，用一个实现了ISqlDeleteBuilder接口的实例产生一条SQL DELETE statement。当IModelMapper.SaveChanges被调用时，该SQL DELETE statement 将被执行。

Tracks a database table delete operation. A SQL DELETE statement will be generated using an instance which has implemented the ISqlDeleteBuilder interface. When IModelMapper.SaveChanges is called, the SQL DELETE statement will be executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackDelete(ISqlDeleteBuilder deleteBuilder, params object[] parameters);
```

**Parameters**

`deleteBuilder` [Appeon.CoreService.Data.ISqlDeleteBuilder](../../ISqlDeleteBuilder/ISqlDeleteBuilder.html)

An interface used to build the SQL DELETE statement.

`parameters` System.Object[]

(Optional) One or more values that you want to use as arguments in the DELETE SQL statement defined in deleteBuilder.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x