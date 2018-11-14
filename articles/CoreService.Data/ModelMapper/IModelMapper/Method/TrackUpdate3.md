

## **IModelMapper.TrackUpdate&#60;TModel>(ISqlUpdateBuilder updateBuilder, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表的修改操作，用一个实现了ISqlUpdateBuilder接口的实例产生一条SQL UPDATE statement。当IModelMapper.SaveChanges被调用时，该SQL UPDATE statement 将被执行。

Tracks a database table update operation. A SQL UPDATE statement will be generated using an instance which has implemented the ISqlUpdateBuilder interface. When IModelMapper.SaveChanges is called, the SQL UPDATE statement will be executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackUpdate(ISqlUpdateBuilder updateBuilder, params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`updateBuilder` [Appeon.CoreService.Data.ISqlUpdateBuilder](../../ISqlUpdateBuilder/ISqlUpdateBuilder.html)

An interface used to build the SQL UPDATE statement.

`parameters` System.Object[]

One or more values that you want to use as arguments in the SQL UPDATE statement defined in updateBuilder.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x