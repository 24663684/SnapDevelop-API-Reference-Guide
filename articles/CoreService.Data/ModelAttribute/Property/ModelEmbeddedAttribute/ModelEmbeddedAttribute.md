## **ModelEmbeddedAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明Model Class中的某一个Property将使用另一个特定的Model Class来进行独立的数据加载或者更新。

Specifies that a property in the model class will use the specified model class to load and update data independently.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.IModelEmbedded](../../../IModelEmbedded/IModelEmbedded.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Property)]
   public class ModelEmbeddedAttribute : Attribute, IModelEmbedded
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [ModelEmbeddedAttribute(Type modelType)](Constructor/ModelEmbeddedAttribute.html) | Initializes a new instance of the ModelEmbeddedAttribute class. |

### **Properties**

|                             | Name                                             | Return Type                                                   | Description                                                         |
| --------------------------- | ------------------------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [CascadeCreate](Property/CascadeCreate.html)     | bool                                                       | Gets or sets whether to insert data to the associated property in the detail model or the granddetail model when the model class is inserting data. |
| ![](~/images/property.jpeg) | [CascadeDelete](Property/CascadeDelete.html)     | bool                                                       | Gets or sets whether to delete data for the associated property in the detail model or the granddetail model when the model class is deleting data. |
| ![](~/images/property.jpeg) | [ModelType](Property/ModelType.html)             | Type                                                       | Gets the type of a model class which the property relies on to load and update data. |
| ![](~/images/property.jpeg) | [ParamValue](Property/ParamValue.html)           | string                                                     | Gets or sets the value of the parameter that is required when loading the data for the current property. |
| ![](~/images/property.jpeg) | [QueryExpression](Property/QueryExpression.html) | string                                                     | Sets the SQL expression parameter that corresponds to the query method of the QuerySelector property. |
| ![](~/images/property.jpeg) | [QuerySelector](Property/QuerySelector.html)     | [QuerySelector](../../../QuerySelector/QuerySelector.html) | Gets or sets the query method to be used when loading the data for the current property. |

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x