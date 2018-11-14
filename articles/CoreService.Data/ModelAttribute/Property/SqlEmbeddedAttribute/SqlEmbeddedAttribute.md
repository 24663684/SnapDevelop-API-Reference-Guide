## **SqlEmbeddedAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明Model Class中的某一个Property将使用特定的raw SQL SELECT Statement来进行的数据加载。

Specifies that a property of the model class will use the specified raw SQL SELECT statement to load data.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlEmbedded](../../../ISqlEmbedded/ISqlEmbedded.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property)]
   public class SqlEmbeddedAttribute : Attribute, ISqlEmbedded
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlEmbeddedAttribute(string rawSql)](Constructor/SqlEmbeddedAttribute.html) | Initializes a new instance of the SqlEmbeddedAttribute class. |

### **Properties**

|                             | Name                                   | Return Type | Description                                                         |
| --------------------------- | -------------------------------------- | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [ParamValue](Property/ParamValue.html) | string   | Gets or sets the value of the parameter that is required when loading the data for the current property. |
| ![](~/images/property.jpeg) | [RawSql](Property/RawSql.html)         | string   | Gets the raw SQL SELECT statement that will be used to load the data for the current property. |

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x