

## **ILoadable.LoadByKey(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Retrieves data according to the primary key defined in a TModel class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  ILoadable<TModel> LoadByKey(params object[] parameters);
```

**Parameters**

`parameters`	System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined by the main table and its primary key(s) in TModel.

**Returns**

Appeon.CoreService.Data.ILoadable&#60;TModel>

Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**

If the SQL query defined in TModel makes query from multiple tables, then this method only retrieves and loads data from the primary table.

### **Examples**



### **Applies to**

.NET Standard 

2.x