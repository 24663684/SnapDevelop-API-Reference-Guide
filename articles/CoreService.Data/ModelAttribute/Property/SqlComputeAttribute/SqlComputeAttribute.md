## **SqlComputeAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Represents a computed column that a property is mapped to. 

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlCompute](../../../ISqlCompute/ISqlCompute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property)]
   public class SqlComputeAttribute : Attribute, ISqlCompute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlComputeAttribute(string expression)](Constructor/SqlComputeAttribute1.html) | Initializes a new instance of the SqlComputeAttribute class. |
| ![](~/images/method.jpeg) | [SqlComputeAttribute(string expression, string alias)](Constructor/SqlComputeAttribute2.html) | Initializes a new instance of the SqlComputeAttribute class. |

### **Properties**

|                             | Name                                       | Return Type | Description                                                         |
| --------------------------- | ------------------------------------------ | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [Alias](Property/Alias.html)               | string   | Gets the alias of the computed column.                       |
| ![](~/images/property.jpeg) | [AliasDefined](Property/AliasDefined.html) | bool     | Gets whether the computed column has an alias.               |
| ![](~/images/property.jpeg) | [Expression](Property/Expression.html)     | string   | Gets the SQL expression which represents the computed column. |
| ![](~/images/property.jpeg) | [Order](Property/Order.html)               | int      | Gets or sets the zero-based order of the computed column the property is mapped to. |
| ![](~/images/property.jpeg) | [TypeName](Property/TypeName.html)         | string   | Gets or sets the data type (specific to the database provider) of the computed column the property is mapped to. |

### **Remarks**

When you define the computed column, the value is calculated by the DBMS when the data is retrieved. 

### **Examples**



### **Applies to**

.NET Standard 

2.x