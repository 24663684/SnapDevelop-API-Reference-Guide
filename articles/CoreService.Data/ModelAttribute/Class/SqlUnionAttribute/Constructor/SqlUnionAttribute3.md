## **SqlUnionAttribute.SqlUnionAttribute(Type modelType, string selectName) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SqlUnionAttribute class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public SqlUnionAttribute(Type modelType, string selectName)
```

**Parameters**

`modelType` System.Type

The type of a model class whose SQL SELECT statement is part of the UNION operator.

`selectName` System.String

modelType中预先定义的Select Name (SqlSelectAttribute.SelectName).

Select Name (SqlSelectAttribute.SelectName) predefined in modelType.

### **Remarks**





### **Applies to**

.NET Standard 

2.x