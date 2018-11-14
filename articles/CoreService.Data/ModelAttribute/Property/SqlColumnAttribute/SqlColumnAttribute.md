## **SqlColumnAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Represents the database column that a property is mapped to. 

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlColumn](../../../ISqlColumn/ISqlColumn.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property)]
   public class SqlColumnAttribute : Attribute, ISqlColumn
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlColumnAttribute(string column)](Constructor/SqlColumnAttribute1.html) | Initializes a new instance of the SqlColumnAttribute class. |
| ![](~/images/method.jpeg) | [SqlColumnAttribute(string tableAlias, string column)](Constructor/SqlColumnAttribute2.html) | Initializes a new instance of the SqlColumnAttribute class. |
| ![](~/images/method.jpeg) | [SqlColumnAttribute(string tableAlias, string column, string columnAlias)](Constructor/SqlColumnAttribute3.html) | Initializes a new instance of the SqlColumnAttribute class. |

### **Properties**

|                             | Name                                                   | Return Type | Description                                                         |
| --------------------------- | ------------------------------------------------------ | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [Column](Property/Column.html)                         | string   | Gets the name of the column the property is mapped to.       |
| ![](~/images/property.jpeg) | [ColumnAlias](Property/ColumnAlias.html)               | string   | Gets the alias of the column the property is mapped to.      |
| ![](~/images/property.jpeg) | [ColumnAliasDefined](Property/ColumnAliasDefined.html) | bool     | Gets whether the column has an alias.                        |
| ![](~/images/property.jpeg) | [Order](Property/Order.html)                           | int      | Gets or sets the zero-based order of the column the property is mapped to. |
| ![](~/images/property.jpeg) | [TableAlias](Property/TableAlias.html)                 | string   | Gets the alias of the table where the column belongs to.     |
| ![](~/images/property.jpeg) | [TableAliasDefined](Property/TableAliasDefined.html)   | bool     | Gets whether the table (where the column belongs to) has an alias. |
| ![](~/images/property.jpeg) | [TypeName](Property/TypeName.html)                     | string   | Gets or sets the data type (specific to the database provider) of the column the property is mapped to. |

### **Remarks**

与.NET提供的System.ComponentModel.DataAnnotations.Schema.ColumnAttribute Class的主要区别在与，增加了对列的别名和表的别名的支持。

Compared to the System.ComponentModel.DataAnnotations.Schema.ColumnAttribute class provided by .NET, the only difference is we support the column alias and the table alias.

如果Model Class中只有一个需要映射的表，且Model class中Properties的Name和数据库中的列名一致(不区分大小写)，则可省略SqlColumnAttribute。

If there is only one table in the model class that needs to be mapped, and the property name of the model class is the same as the column name of the database table (case is insensitive), then the SqlColumn attribute can be ignored.

### **Examples**



### **Applies to**

.NET Standard 

2.x