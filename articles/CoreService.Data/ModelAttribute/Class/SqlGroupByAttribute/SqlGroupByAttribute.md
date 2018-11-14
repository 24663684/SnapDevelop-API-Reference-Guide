## **SqlGroupByAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明一个Model Class将把查询结果划分为多个行组。

Denotes that a model class should divide the query result into groups of rows.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlGroupBy](../../../ISqlGroupBy/ISqlGroupBy.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class SqlGroupByAttribute : Attribute, ISqlGroupBy
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlGroupByAttribute(params string[] expressions)](Constructor/SqlGroupByAttribute.html) | Initializes a new instance of the SqlGroupByAttribute class. |

### **Properties**

|                             | Name                                                   | Return Type                  | Description                                                         |
| --------------------------- | ------------------------------------------------------ | ------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [GroupByExpressions](Property/GroupByExpressions.html) | IReadOnlyList&#60;string> | Gets one or more raw SQL expressions in the GROUP BY clause without the keyword GROUP BY. |

### **Remarks**

SqlGroupByAttribute 指明一个Model Class将在SQL SELECT语句中使用GROUP BY Clause来将查询结果划分为多个行组。

The SqlGroupBy attribute denotes that a model class should use a GROUP BY Clause in the SQL SELECT statement to divide the query result into several groups of rows.

### **Examples**



### **Applies to**

.NET Standard 

2.x