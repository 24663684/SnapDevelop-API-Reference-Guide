## **SqlOrderByAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明当一个Model Class加载数据时如何对查询的结果集进行排序。

Specifies how a model class sorts the result set when loading data.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlOrderBy](../../../ISqlOrderBy/ISqlOrderBy.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class SqlOrderByAttribute : Attribute, ISqlOrderBy
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlOrderByAttribute(params string[] expressions)](Constructor/SqlOrderByAttribute.html) | Initializes a new instance of the SqlOrderByAttribute class. |

### **Properties**

|                             | Name                           | Return Type                                                   | Description                                                         |
| --------------------------- | ------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [OnType](Property/OnType.html) | [SqlJoinOnType](../../../SqlJoinOnType/SqlJoinOnType.html) | Gets one or more raw SQL expressions in the ORDER BY clause without the keyword ORDER BY. |

### **Remarks**

SqlOrderByAttribute指明一个Model Class将在SQL SELECT语句中使用ORDER BY Clause来对查询的结果集进行排序。

The SqlOrderBy attribute denotes that a model class should use the ORDER BY clause in the SQL SELECT statement to sort the result set of the query.

### **Examples**



### **Applies to**

.NET Standard 

2.x