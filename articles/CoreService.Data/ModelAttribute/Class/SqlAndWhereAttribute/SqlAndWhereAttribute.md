## **SqlAndWhereAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class已有的search condition的基础上, 指定需要同时满足的另外一个search condition。一个Model class中允许指定多个SqlAndWhereAttribute实例。

Sets an additional search condition on top of the existing search condition in the model class. One or more SqlAndWhere attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlWhereAttribute](../SqlWhereAttribute/SqlWhereAttribute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlAndWhereAttribute : SqlWhereAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlAndWhereAttribute(string rawCondition)](Constructor/SqlAndWhereAttribute1.html) | Initializes a new instance of the SqlAndWhereAttribute class. |
| ![](~/images/method.jpeg) | [SqlAndWhereAttribute(string left, string right)](Constructor/SqlAndWhereAttribute2.html) | Initializes a new instance of the SqlAndWhereAttribute class. |

### **Remarks**

该特性必须同ModelAttribute.SqlWhereAttribute一同使用。

The SqlAndWhere attribute must be used together with ModelAttribute.SqlWhereAttribute.

SqlAndWhereAttribute 指明一个Model Class将在SQL SELECT语句中的WHERE Clause中添加AND logical operator and another search condition。

The SqlAndWhere attribute denotes that a model class should add an AND logical operator and another search condition in the WHERE clause of the SQL SELECT statement.

### **Examples**



### **Applies to**

.NET Standard 

2.x