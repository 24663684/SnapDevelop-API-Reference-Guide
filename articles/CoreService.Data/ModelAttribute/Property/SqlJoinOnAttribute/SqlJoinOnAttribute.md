## **SqlJoinOnAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定联接一个joined table的联接条件。

Specifies the condition for joining a table.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlJoinOn](../../../ISqlJoinOn/ISqlJoinOn.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property, AllowMultiple = true)]
   public class SqlJoinOnAttribute : Attribute, ISqlJoinOn
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlJoinOnAttribute(string tableAlias, string joinColumn)](Constructor/SqlJoinOnAttribute.html) | Initializes a new instance of the SqlJoinOnAttribute class. |

### **Properties**

|                             | Name                                     | Return Type                                                   | Description                                                         |
| --------------------------- | ---------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [JoinColumn](Property/JoinColumn.html)   | string                                                     | Gets the alias of the column of the joined table.            |
| ![](~/images/property.jpeg) | [OnType](Property/OnType.html)           | [SqlJoinOnType](../../../SqlJoinOnType/SqlJoinOnType.html) | Returns the logical operator of the join conditions for the current property. |
| ![](~/images/property.jpeg) | [SqlOperator](Property/SqlOperator.html) | [SqlOperator](../../../SqlOperator/SqlOperator.html)       | Gets or sets the operator for joining the table.             |
| ![](~/images/property.jpeg) | [TableAlias](Property/TableAlias.html)   | string                                                     | Gets the alias of the joined table.                          |

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x