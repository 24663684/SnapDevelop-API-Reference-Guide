## **SqlUnionAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明一个Model Class将两个或者更多个查询的结果合并为单个结果集。一个Model class中允许指定多个SqlUnionAttribute 实例。

Denotes that a model class should combine the results of two or more queries into one single result. One or more SqlUnion attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

System.Attribute

[Appeon.CoreService.Data.ISqlUnion](../../../ISqlUnion/ISqlUnion.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlUnionAttribute : Attribute, ISqlUnion
```

### **Constructors**

|                           | Name                                                         | Description                                                       |
| ------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlUnionAttribute(string rawSql)](Constructor/SqlUnionAttribute1.html) | Initializes a new instance of the SqlUnionAttribute class. |
| ![](~/images/method.jpeg) | [SqlUnionAttribute(Type modelType)](Constructor/SqlUnionAttribute2.html) | Initializes a new instance of the SqlUnionAttribute class. |
| ![](~/images/method.jpeg) | [SqlUnionAttribute(Type modelType, string selectName)](Constructor/SqlUnionAttribute3.html) | Initializes a new instance of the SqlUnionAttribute class. |

### **Properties**

|                             | Name                                   | Return Type | Description                                                         |
| --------------------------- | -------------------------------------- | -------- | ------------------------------------------------------------ |
| ![](~/images/property.jpeg) | [IsRawSql](Property/IsRawSql.html)     | bool     | Gets whether a raw SQL has been specified for the union operation. |
| ![](~/images/property.jpeg) | [ModelType](Property/ModelType.html)   | Type     | Gets the type of the model that is specified for the union operator. |
| ![](~/images/property.jpeg) | [RawSql](Property/RawSql.html)         | string   | Gets the raw SQL specified for the union operator.           |
| ![](~/images/property.jpeg) | [SelectName](Property/SelectName.html) | string   | Gets the Select Name (SqlSelectAttribute.SelectName) predefined in the model type specified by the union operator. |
| ![](~/images/property.jpeg) | [UnionAll](Property/UnionAll.html)     | bool     | Gets or sets whether to use UNION ALL.                       |

### **Remarks**

SqlUnionAttribute 指明一个Model Class将在SQL SELECT语句中使用UNION operator来将两个或者更多个查询的结果合并为单个结果集。

The SqlUnion attribute denotes that a model class should use an UNION operator in the SQL SELECT statement to combine the results of two or more queries into one single result.

### **Examples**



### **Applies to**

.NET Standard 

2.x