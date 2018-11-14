

## **IModelMapper.Load&#60;TModel>(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据TModel中定义的SQL检索规则检索数据。

Retrieves data according to the SQL query defined in a TModel class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public ILoadable<TModel> Load<TModel>(params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

**Parameters**

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in TModel.

**Returns**

[Appeon.CoreService.Data.ILoadable&#60;TModel>](../../ILoadable/ILoadable.html)

返回ILoadable&#60;TModel>接口，可使用该接口的 Method进一步获取数据结果集，或者进行嵌套查询等操作。

Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**



### **Examples**





### **Applies to**

.NET Standard 

2.x 	