

## **ILoadable.Load(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

 Retrieves data according to the SQL query defined in a TModel class. 

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  ILoadable<TModel> Load(params object[] parameters);
```

**Parameters**

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in TModel.

**Returns**

Appeon.CoreService.Data.ILoadable&#60;TModel>

Returns the ILoadable<TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**

Load Method会根据TModel中应用的特性生成查询，并且传入TModel定义的查询参数。

The ILoadable.Load method will generate the SQL query according to the attribute applied to TModel and pass in the query parameter defined in TModel.

### **Examples**





### **Applies to**

.NET Standard 

2.x