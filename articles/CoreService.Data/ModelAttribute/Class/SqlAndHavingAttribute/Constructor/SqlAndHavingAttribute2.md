## **SqlAndHavingAttribute.SqlAndHavingAttribute(string left, string right) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SqlAndHavingAttribute class. 

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public SqlAndHavingAttribute(string left, string right):base(left, right)
```

**Parameters**

`left`	System.String

The raw SQL expression on the left of the operator property.

If the operator property is not specified, the operator defaults to "=".

`right` System.String

The raw SQL expression on the right of the operator property.

### **Remarks**



### **Applies to**

.NET Standard 

2.x