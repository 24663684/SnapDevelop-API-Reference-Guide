## **SqlWhereAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定一个Model Class在加载数据时结果集需要满足的条件。

Sets the condition for the result set when a model class loads the data.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class SqlWhereAttribute : Attribute
```

### **Constructors**

|                           | Name                                                         | Description                                                       |
| ------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlWhereAttribute(string rawCondition)](Constructor/SqlWhereAttribute1.html) | Initializes a new instance of the SqlWhereAttribute class. |
| ![](~/images/method.jpeg) | [SqlWhereAttribute(string left, string right)](Constructor/SqlWhereAttribute2.html) | Initializes a new instance of the SqlWhereAttribute class. |

### **Properties**

|                             | Name                                                     | Return Type                                             | Description                                                         |
| --------------------------- | -------------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [Left](Property/Left.html)                               | string                                               | Gets the raw SQL expression on the left of the operator property. |
| ![](~/images/property.jpeg) | [Operator](Property/Operator.html)                       | [SqlOperator](../../../SqlOperator/SqlOperator.html) | Gets or sets the operator used in the WHERE clause of the raw SQL. |
| ![](~/images/property.jpeg) | [RawCondition](Property/RawCondition.html)               | string                                               | Gets the raw SQL search condition in the WHERE clause without the keyword WHERE. |
| ![](~/images/property.jpeg) | [RawConditionDefined](Property/RawConditionDefined.html) | bool                                                 | Gets whether the current instance of the SqlWhere attribute is initialized by a raw SQL search condition. |
| ![](~/images/property.jpeg) | [Right](Property/Right.html)                             | string                                               | Gets the raw SQL expression on the right of the operator property. |

### **Remarks**

SqlWhereAttribute的作用相当在Model class产生的SQL SELECT语句中使用WHERE Clause来定义结果集需要满足的条件。

The SqlWhere attribute is equivalent to adding a WHERE clause (that defines the condition for the result set) to the SQL SELECT statement of the model class.

### **Examples**



### **Applies to**

.NET Standard 

2.x