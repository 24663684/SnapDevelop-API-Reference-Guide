

## **IModelMapper.TrackSqlCUD(string sqlText, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表的新增，修改或者删除的操作，用一条生写的SQL INSERT, UPDATE, or DELETE statement。当IModelMapper.SaveChanges被调用时，该SQL statement 将被执行。

Tracks a database table operation (insert, update or delete) using a raw SQL statement (INSERT, UPDATE, or DELETE). When IModelMapper.SaveChanges is called, the SQL statement will be executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackSqlCUD(string sqlText, params object[] parameters);
```

**Parameters**

`sqlText` System.String

An SQL INSERT, UPDATE, or DELETE statement. 

可以使用:或者@号开头标识来表示SQL中需要的参数。

Use : or @ symbol at the beginning to represent the parameter required by the SQL statement.

`parameters` System.Object[]

SQL中需要的arguments，需要保证argument的顺序与sqlText中参数的顺序一致。

The arguments required by the SQL statement. The order of arguments here must be the same as the order of arguments in sqlText.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x