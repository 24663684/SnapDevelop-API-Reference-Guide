## **DistinctAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明一个Model Class将在加载数据时将去除重复值。

Denotes that a model class should remove the duplicate values when loading data.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class DistinctAttribute : Attribute
```

### **Constructors**

|                           | Name                                                      | Description                                                       |
| ------------------------- | --------------------------------------------------------- | ---------------------------------------------------------- |
| ![](~/images/method.jpeg) | [DistinctAttribute()](Constructor/DistinctAttribute.html) | Initializes a new instance of the DistinctAttribute class. |

### **Remarks**

DistinctAttribute的作用相当在Model class产生的SQL SELECT语句中add DISTINCT to removes duplicate values.

The Distinct attribute is equivalent to add DISTINCT in the SQL SELECT statement to removes duplicate values.

### **Examples**



### **Applies to**

.NET Standard 

2.x