## **SqlParameterAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class内定义一个指定了Name和Type的Parameter。

Defines a parameter with name and type in the model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlParameter](../../../ISqlParameter/ISqlParameter.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlParameterAttribute : Attribute, ISqlParameter
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlParameterAttribute(string name, Type dataType)](Constructor/SqlParameterAttribute.html) | Initializes a new instance of the SqlParameterAttribute class. |

### **Properties**

|                             | Name                               | Return Type | Description                                 |
| --------------------------- | ---------------------------------- | -------- | ------------------------------------ |
| ![](~/images/property.jpeg) | [DataType](Property/DataType.html) | Type     | Gets the data type of the parameter. |
| ![](~/images/property.jpeg) | [Name](Property/Name.html)         | string   | Gets the name of the parameter.      |

### **Remarks**

可以在为该Model Class中其他特性的允许编写SQL Expression的参量中通过Name引用该Parameter，格式: $Param(paramName) 或者:paramName.

The parameter can be referenced by its name in the SQL expression parameter for the other attributes in the model class. The format to make reference: $Param(paramName) or :paramName.

### **Examples**



### **Applies to**

.NET Standard 

2.x