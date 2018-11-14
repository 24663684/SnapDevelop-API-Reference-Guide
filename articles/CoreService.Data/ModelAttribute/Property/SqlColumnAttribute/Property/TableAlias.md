## **SqlColumnAttribute.TableAlias Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取表示该column所属的表的别名。

Gets the alias of the table where the column belongs to.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public string TableAlias { get; }
```

**Property Value**

System.String

column所属的表的别名，需要与Model class中FromTableAttribute实例或者JoinTableAttribute实例的AliasProperties一致。

The alias of the table where the column belongs to. It must be the same as the Alias property of the FromTable attribute or the JoinTable attribute of the model class.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x