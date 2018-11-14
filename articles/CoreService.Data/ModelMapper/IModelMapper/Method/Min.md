

## **IModelMapper.Min&#60;TModel>(string expression, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据一个Model中预先定义的检索条件来获取指定SQL Expression对应的最小值。

Gets the minimum value for the specified SQL expression according to the retrieval criteria specified in a model.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public object Min<TModel>(string expression, params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

**Parameters**

`expression` System.String

用于计算最小值的SQL Expression字符串。

A string of SQL expression used to compute the minimum value.

 `parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in TModel.

**Returns**

System.Object

检索返回的最小值，其数据类型是SQL执行后返回值的数据类型。

The minimum value of the retrieved data. Its data type is determined by the return value of the SQL expression.

### **Remarks**

参数expression所包含的SQL Expression字符串，将最终被用于SQL的MIN()函数中。因此SQL Expression字符串必须满足SQL规范，否则将抛出异常。

The `expression` parameter contains the string of a SQL expression which will be used by the SQL MIN() function, therefore, the SQL expression string must comply with the SQL conventions, otherwise, exceptions may be thrown.

由于该 Method仅返回首行首列数据，请避免在TModel的定义中存在分组时使用。

This method only returns the data of the first column in the first row of the retrieved data, therefore, please avoid using this method when groups are defined in TModel.

### **Examples**





### **Applies to**

.NET Standard 

2.x