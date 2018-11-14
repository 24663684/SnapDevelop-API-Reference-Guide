## **JoinTableAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定一个Model class中使用的joined table。一个Model class中允许指定多个JoinTableAttribute 实例。

Sets the joined table to be used in a model class. Multiple JoinTable attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.ComponentModel.DataAnnotations.Schema.TableAttribute

[Appeon.CoreService.Data.IJoinTable](../../../IJoinTable/IJoinTable.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class JoinTableAttribute : TableAttribute, IJoinTable
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [JoinTableAttribute(string name)](Constructor/JoinTableAttribute1.html) | Initializes a new instance of the JoinTableAttribute class. |
| ![](~/images/method.jpeg) | [JoinTableAttribute(string alias, string name)](Constructor/JoinTableAttribute2.html) | Initializes a new instance of the JoinTableAttribute class. |

### **Properties**

|                             | Name                                       | Return Type                                             | Description                                                         |
| --------------------------- | ------------------------------------------ | ---------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [Alias](Property/Alias.html)               | string                                               | Gets the alias of the specified joined table.                |
| ![](~/images/property.jpeg) | [AliasDefined](Property/AliasDefined.html) | bool                                                 | Gets whether the joined table has an alias.                  |
| ![](~/images/property.jpeg) | [Id](Property/Id.html)                     | int                                                  | Gets the ID of the joined table in the model class.          |
| ![](~/images/property.jpeg) | [JoinType](Property/JoinType.html)         | [SqlJoinType](../../../SqlJoinType/SqlJoinType.html) | Gets or sets the type of join operation in the FROM clause.  |
| ![](~/images/property.jpeg) | [OnRaw](Property/OnRaw.html)               | string                                               | Gets or sets the raw SQL condition on which the join is based. |

### **Remarks**

JoinTableAttribute 相当于允许将SQL Select语句的INNER JOIN, FULL OUTER JOIN, LEFT OUTER JOIN, RIGHT OUTER JOIN等join types作用于Model上来定义多个表的联结关系。

The JoinTable attribute is equivalent to applying the join type (INNER JOIN, FULL OUTER JOIN, LEFT OUTER JOIN, RIGHT OUTER JOIN etc.) of the SQL Select statement to the model so as to define the joining relationship between tables.

### **Examples**



### **Applies to**

.NET Standard 

2.x