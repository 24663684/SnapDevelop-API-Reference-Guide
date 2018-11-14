## **TopAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明一个Model Class将限制返回的结果行数。

Denotes that a model class should limit the rows returned.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class TopAttribute : Attribute
```

### **Constructors**

|                           | Name                                                      | Description                                                  |
| ------------------------- | --------------------------------------------------------- | ----------------------------------------------------- |
| ![](~/images/method.jpeg) | [TopAttribute(int number)](Constructor/TopAttribute.html) | Initializes a new instance of the TopAttribute class. |

### **Properties**

|                             | Name                             | Return Type | Description                                            |
| --------------------------- | -------------------------------- | -------- | ----------------------------------------------- |
| ![](~/images/property.jpeg) | [TopRows](Property/TopRows.html) | int      | Gets the maximum number of rows to be returned. |

### **Remarks**

TopAttribute 指明一个Model Class将在SQL SELECT语句中添加TOP Clause去限制返回的结果行数。

The Top attribute denotes that a model class should adds a TOP clause to the SQL SELECT statement to limit the rows returned.

### **Examples**



### **Applies to**

.NET Standard 

2.x