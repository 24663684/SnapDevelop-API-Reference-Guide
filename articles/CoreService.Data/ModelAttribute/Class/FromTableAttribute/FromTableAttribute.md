## **FromTableAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定一个Model类映射到的数据库表。一个Model Class中允许指定多个FromTableAttribute实例。

Specifies the database table that a model class is mapped to. Multiple FromTable attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.ComponentModel.DataAnnotations.Schema.TableAttribute

[Appeon.CoreService.Data.IFromTable](../../../IFromTable/IFromTable.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class FromTableAttribute : TableAttribute, IFromTable
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [FromTableAttribute(string name)](Constructor/FromTableAttribute1.html) | Initializes a new instance of the FromTableAttribute class. |
| ![](~/images/method.jpeg) | [FromTableAttribute(string alias, string name)](Constructor/FromTableAttribute2.html) | Initializes a new instance of the FromTableAttribute class. |

### **Properties**

|                             | Name                                       | Return Type | Description                                                         |
| --------------------------- | ------------------------------------------ | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [Alias](Property/Alias.html)               | string   | Gets the alias of the specified database table.              |
| ![](~/images/property.jpeg) | [AliasDefined](Property/AliasDefined.html) | bool     | Gets whether the specified database table has an alias.      |
| ![](~/images/property.jpeg) | [Id](Property/Id.html)                     | int      | Gets the ID of the database table specified in the model class. |
| ![](~/images/property.jpeg) | [WhereRaw](Property/WhereRaw.html)         | string   | Gets or sets the raw Where clause for the specified database table. |

### **Remarks**

FromTableAttibute的作用相当于SQL SELECT语句中的FROM Clause中的数据库表,可以为一个Model类应用多个FromTable特性以便在一个Model中检索多张表的数据。  

The FromTable attribute is equivalent to the database table in the FROM Clause of the SQL SELECT statement. One or more FromTable attributes can be applied to one model class so as to retrieving from one or more database tables in one model.

当没有TableAtrribute 并且一个或者多个FromTableAtrributes被用于一个Model Class时，第一个FromTableAttibute也指明了Model Class在执行SQL DML时使用的唯一的表。

When no Table attribute is applied, and one or more FromTable attributes are being applied to a model class, the first FromTable attribute denotes the only one database table that the model class should use when executing the SQL DML. 



### **Examples**



### **Applies to**

.NET Standard 

2.x