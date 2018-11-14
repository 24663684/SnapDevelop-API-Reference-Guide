## **SubQueryAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class内定义一个指定了Name的subquery。

Defines a subquery in the model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISubQuery](../../ISubQuery/ISubQuery.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SubQueryAttribute : Attribute, ISubQuery
```

### **Constructors**

|                           | Name                                                         | Description                                                       |
| ------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SubQueryAttribute(string name, string rawSql)](Constructor/SubQueryAttribute1.html) | Initializes a new instance of the SubQueryAttribute class. |
| ![](~/images/method.jpeg) | [SubQueryAttribute(string name, Type modelType)](Constructor/SubQueryAttribute2.html) | Initializes a new instance of the SubQueryAttribute class. |
| ![](~/images/method.jpeg) | [SubQueryAttribute(string name, Type modelType, string selectName)](Constructor/SubQueryAttribute3.html) | Initializes a new instance of the SubQueryAttribute class. |

### **Properties**

|                             | Name                                   | Return Type | Description                                                         |
| --------------------------- | -------------------------------------- | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [IsRawSql](Property/IsRawSql.html)     | bool     | Gets whether a raw SQL has been specified for the subquery.  |
| ![](~/images/property.jpeg) | [ModelType](Property/ModelType.html)   | Type     | Gets the type of the model that is specified for the subquery. |
| ![](~/images/property.jpeg) | [Name](Property/Name.html)             | string   | Gets the name of the subquery.                               |
| ![](~/images/property.jpeg) | [RawSql](Property/RawSql.html)         | string   | Gets the raw SQL that is specified for the subquery.         |
| ![](~/images/property.jpeg) | [SelectName](Property/SelectName.html) | string   | Gets the Select Name (SqlSelectAttribute.SelectName) that is predefined in the model type. |

### **Remarks**

可以在为该Model Class中其他特性的允许编写SQL Expression的参量中通过Name引用该subquery, 格式: $SubQuery(Name).

The subquery can be referenced by its name in the SQL expression parameter for the other attributes in the model class. The format to make reference: $SubQuery(Name).

### **Examples**



### **Applies to**

.NET Standard 

2.x