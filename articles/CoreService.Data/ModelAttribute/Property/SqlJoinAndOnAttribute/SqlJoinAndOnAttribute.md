## **SqlJoinAndOnAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定联接一个joined table的联接条件，使用AND操作符。

Specifies the condition for joining a table, using the AND operator.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlJoinOnAttribute](../SqlJoinOnAttribute/SqlJoinOnAttribute.html)

### **Syntax**

```c#
   public class SqlJoinAndOnAttribute : SqlJoinOnAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlJoinAndOnAttribute(string tableId, string joinColumn)](Constructor/SqlJoinAndOnAttribute.html) | Initializes a new instance of the SqlJoinAndOnAttribute class. |

### **Properties**

|                             | Name                           | Return Type                                                   | Description                                                         |
| --------------------------- | ------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [OnType](Property/OnType.html) | [SqlJoinOnType](../../../SqlJoinOnType/SqlJoinOnType.html) | Returns the logical operator of the join conditions for the current property. |

### **Remarks**

待定。

### **Examples**



### **Applies to**

.NET Standard 

2.x