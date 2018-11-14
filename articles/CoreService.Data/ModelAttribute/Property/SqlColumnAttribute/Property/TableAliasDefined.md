## **SqlColumnAttribute.TableAliasDefined Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取是否已定义列所属的表的别名。

Gets whether the table (where the column belongs to) has an alias.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
    public bool TableAliasDefined => !string.IsNullOrWhiteSpace(this.TableAlias);
```

**Property Value**

System.Boolean

True, 已定义列所属的表的别名；

True: an alias has been defined for the table (where the column belongs to)

False,未定义列所属的表的别名。

False: no alias has been defined for the table (where the column belongs to)

The default is False.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x