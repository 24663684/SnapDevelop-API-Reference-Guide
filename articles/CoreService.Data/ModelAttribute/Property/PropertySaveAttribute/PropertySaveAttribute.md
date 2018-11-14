## **PropertySaveAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定一个Properties在保存数据到数据库时采用的策略。

Specifies the strategy to be used when saving the data for a property to the database.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.IPropertySave](../../../IPropertySave/IPropertySave.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property)]
   public class PropertySaveAttribute : Attribute, IPropertySave
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [PropertySaveAttribute(SaveStrategy saveStrategy)](Constructor/PropertySaveAttribute.html) | Initializes a new instance of the PropertySaveAttribute class. |

### **Properties**

|                             | Name                                       | Return Type                                                | Description                                                         |
| --------------------------- | ------------------------------------------ | ------------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [SaveStrategy](Property/SaveStrategy.html) | [SaveStrategy](../../../SaveStrategy/SaveStrategy.html) | Gets the strategy that is used when saving the data for the current property to the database. |

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x