

## **ILoadable.Load(ISqlQueryBuilder queryBuilder, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Retrieves data according to the SQL query defined in the SqlQueryBuilder instance.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  ILoadable<TModel> Load(ISqlQueryBuilder queryBuilder, params object[] parameters);
```

**Parameters**

`queryBuilder` [Appeon.CoreService.Data.ISqlQueryBuilder]()

A SqlQueryBuilder instance which can be used to overwrite the static SQL query defined in a Model class, so as to perform dynamic retrieval.

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in queryBuilder.

**Returns**

Appeon.CoreService.Data.ILoadable&#60;TModel>

Returns the ILoadable<TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**

Load Method会使用SqlQueryBuilder构建的查询，并且传入查询所需要参数。

The ILoadable.Load method will use the SQL query constructed by SqlQueryBuilder and pass in the parameter required by the query.

### **Examples**



### **Applies to**

.NET Standard 

2.x