

## **IModelMapper.Count&#60;TModel>(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据TModel中定义的检索条件来检索数据库结果集的行数。

Gets the number of rows in the result set retrieved according to the criteria specified in a TModel class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public int Count<TModel>(params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

**Parameters**

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in TModel.

**Returns**

System.Int32

返回数据库结果集的行数。

Returns the number of rows in the database result set.

### **Remarks**

该 Method内部使用到了SQL的COUNT()函数。

This method uses the SQL COUNT() function internally.

由于该 Method仅返回首行首列数据，请避免在TModel的定义中存在分组时使用。

This method only returns the data of the first column in the first row of the retrieved data, therefore, please avoid using this method when groups are defined in TModel.

### **Examples**



### **Applies to**

.NET Standard 

2.x