## **SetValueAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

已通过当前Properties定义Model Class嵌套关系后，指明在Model Class新增或者修改数据库后，将把本级Model Class的某一个Properties的值设置到下一级Model Class的某一个Properties。一个Property中允许指定多个SetValueAttribute实例。

Specifies that when there is an insert or update operation in the master model, set the property value of the master model to the associate property of the detail model, when working with the master-detail models. One property is allowed to apply multiple SetValue attributes.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISetValue](../../../ISetValue/ISetValue.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property, AllowMultiple = true)]
   public class SetValueAttribute : Attribute, ISetValue
```

### **Constructors**

|                           | Name                                                         | Description                                                       |
| ------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SetValueAttribute( string source,string target)](Constructor/SetValueAttribute1.html) | Initializes a new instance of the SetValueAttribute class. |
| ![](~/images/method.jpeg) | [SetValueAttribute(string source,string target,SetValueStrategy setValueStrategy)](Constructor/SetValueAttribute2.html) | Initializes a new instance of the SetValueAttribute class. |
| ![](~/images/method.jpeg) | [SetValueAttribute(string source, string target,  ModelSelector modelSelector)](Constructor/SetValueAttribute3.html) | Initializes a new instance of the SetValueAttribute class. |

### **Properties**

|                             | Name                                               | Return Type                                                     | Description                                                         |
| --------------------------- | -------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [ModelSelector](Property/ModelSelector.html)       | [ModelSelector](../../../ModelSelector/ModelSelector.html)   | Gets the ModelSelector enumerated value which determines whether to set value by the data state in the embedded model. |
| ![](~/images/property.jpeg) | [SetValueStrategy](Property/SetValueStrategy.html) | [SetValueStrategy](../../../SetValueStrategy/SetValueStrategy.html) | Gets the SetValueStrategy enumerated value which determines when to set value. |
| ![](~/images/property.jpeg) | [Source](Property/Source.html)                     | string                                                       | Gets the string that represents a property in the model class at the same level. |
| ![](~/images/property.jpeg) | [Target](Property/Target.html)                     | string                                                       | Gets the string that represents a property in the model class at one level lower. |

### **Remarks**

SetValueAttribute 需要和ModelEmbeddedAttribute一同使用。

The SetValue attribute must be used together with the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute.

### **Examples**



### **Applies to**

.NET Standard 

2.x