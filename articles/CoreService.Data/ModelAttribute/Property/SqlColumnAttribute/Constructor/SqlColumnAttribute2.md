## **SqlColumnAttribute.SqlColumnAttribute(string tableAlias, string column) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SqlColumnAttribute class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public SqlColumnAttribute(string tableAlias, string column)
```

**Parameters**

`tableAlias`	System.String

表示该column所属的表的别名，需要与Model class中FromTableAttribute实例或者JoinTableAttribute实例的AliasProperties一致。

The alias of the table where the column belongs to. This alias must be the same as the Alias property of the FromTable attribute or the JoinTable attribute of the model class.

`column` System.String

The name of the column the property is mapped to.

### **Remarks**



### **Applies to**

.NET Standard 

2.x