## **SqlAndWhereAttribute.SqlAndWhereAttribute(string rawCondition) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SqlAndWhereAttribute class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public SqlAndWhereAttribute(string rawCondition): base(rawCondition)
```

**Parameters**

`rawCondition` System.String

不含AND操作符的生写的WHERE子句中SQL查询条件。

A raw SQL search condition in the WHERE clause without the AND operator.

### **Remarks**



### **Applies to**

.NET Standard 

2.x