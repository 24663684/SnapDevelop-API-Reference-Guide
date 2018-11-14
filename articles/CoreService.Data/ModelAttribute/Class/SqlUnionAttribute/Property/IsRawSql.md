## **SqlUnionAttribute.IsRawSql Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取是否为Union operater指定了raw SQL. 

Gets whether a raw SQL has been specified for the union operation.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
    public bool IsRawSql { get; }
```

**Property Value**

System.Boolean

True, 为Union operator指定了raw SQL.;

True: a raw SQL has been specified for the union operation.

False, 为Union operator指定了Model.

False: a Model has been specified for the union operation.

### **Remarks**

待定。

### **Examples**



### **Applies to**

.NET Standard 

2.x