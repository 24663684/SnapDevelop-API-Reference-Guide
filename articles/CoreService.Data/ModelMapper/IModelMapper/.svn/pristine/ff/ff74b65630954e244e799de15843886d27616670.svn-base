

## **IModelMapper.LoadByKey&#60;TModel>(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据TModel中定义的主键检索数据。

Retrieves data according to the primary key defined in a TModel class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public ILoadable<TModel> LoadByKey<TModel>(params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

**Parameters**

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined by the main table and its primary key(s) in TModel.

**Returns**

[Appeon.CoreService.Data.ILoadable&#60;TModel>](../../ILoadable/ILoadable.html)

返回ILoadable&#60;TModel>接口，可使用该接口的 Method进一步获取数据结果集，或者进行嵌套查询等操作。

Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**

如果TModel中定义的SQL查询是多表查询，那么该 Method仅会检索并得到主表的数据。

If the SQL query defined in TModel makes query from multiple tables, then this method only retrieves and loads data from the primary table.

### **Examples**





### **Applies to**

.NET Standard 

2.x