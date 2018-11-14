## **UpdateWhereStrategyAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定Model Class将在执行数据库更新时将哪些列将作为查询条件。

Specifies the column(s) to be used as search condition when the model class is performing updates to the database.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.IUpdateWhereStrategy](../../../IUpdateWhereStrategy/IUpdateWhereStrategy.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class UpdateWhereStrategyAttribute : Attribute, IUpdateWhereStrategy
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [UpdateWhereStrategyAttribute(UpdateWhereStrategy strategy)](Constructor/UpdateWhereStrategyAttribute.html) | Initializes a new instance of the UpdateWhereStrategyAttribute class. |

### **Properties**

|                             | Name                                                     | Return Type                                                     | Description                                                         |
| --------------------------- | -------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [UpdateWhereStrategy](Property/UpdateWhereStrategy.html) | [UpdateWhereStrategy](../../../UpdateWhereStrategy/UpdateWhereStrategy.html) | Gets the strategy that which column(s) will be included in the WHERE clause of the UPDATE statement. |

### **Remarks**

The UpdateWhereStrategy attribute indicates the strategy that which column(s) will be included in the WHERE clause of the SQL UPDATE statement for a model class.

如果没有为某个Model Class指定UpdateWhereStrategyAttribute, 将默认采用UpdateWhereStrategy.KeyColumns (WHERE statement only including key columns).

If no UpdateWhereStrategy attribute is applied to a model class, the enumaration value UpdateWhereStrategy.KeyColumns (WHERE statement only includes key columns) will be used by default.

### **Examples**



### **Applies to**

.NET Standard 

2.x