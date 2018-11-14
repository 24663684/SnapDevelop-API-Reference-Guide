

## **IModelMapper.ScalarByKey&#60;TModel, TValue>(string expression, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据TModel中定义的主键来检索指定的SQL Expression的第一行的第一列数据。

Retrieves data of the first column in the first row for the specified SQL expression according to the primary key in a TModel class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public TValue ScalarByKey<TModel, TValue>(string expression, params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

`TValue`

The type of the value retrieved.

**Parameters**

`expression` System.String

用于获取第一行的第一列数据的SQL Expression字符串。

A string of SQL expression used to get data of the first column in the first row.

 `parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined by the main table and its primary key(s) in TModel.

**Returns**

System.TValue

检索返回的第一行的第一列数据，其数据类型是SQL执行后返回值的数据类型。

Returns the data of the first column in the first row of the retrieved data. Its data type is determined by the return value of the SQL expression.

### **Remarks**

需要确保按指定的检索条件得到的结果集至少有一行记录，否则将抛出异常。

At least one data row must be retrieved by the specified criteria, otherwise exceptions will be thrown.

### **Examples**



### **Applies to**

.NET Standard 

2.x