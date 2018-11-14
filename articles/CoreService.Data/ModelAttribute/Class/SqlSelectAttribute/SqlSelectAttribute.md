## **SqlSelectAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class内定义一个指定了Name的select list, to decide which columns to be selected from the result set. The select list is a series of expressions separated by commas.

Defines a select list in the model class, to decide which columns to be selected from the result set. The select list is a series of expressions separated by commas.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlSelect](../../../ISqlSelect/ISqlSelect.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlSelectAttribute : Attribute, ISqlSelect
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlSelectAttribute(string selectName)](Constructor/SqlSelectAttribute.html) | Initializes a new instance of the SqlSelectAttribute class. |

### **Properties**

|                             | Name                                   | Return Type | Description                                                         |
| --------------------------- | -------------------------------------- | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [RawSelect](Property/RawSelect.html)   | string   | Gets or sets the raw SQL select list that decides which columns to be selected from the result set. |
| ![](~/images/property.jpeg) | [SelectName](Property/SelectName.html) | string   | Gets the name of the select list.                            |

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x