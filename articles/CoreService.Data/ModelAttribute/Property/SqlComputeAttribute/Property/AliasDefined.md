## **SqlComputeAttribute.AliasDefined Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取是否已定义the alias of the computed column.

Gets whether the computed column has an alias.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public bool AliasDefined => !string.IsNullOrWhiteSpace(this.Alias);
```

**Property Value**

System.Boolean

True, 已定义the alias of the computed column;

True: an alias has been defined for the computed column.

False, 未定义the alias of the computed column.

False: no alias has been defined for the computed column.

The default is False.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x