## **SqlOrWhereAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class已有的search condition的基础上, 指定另外一个search condition,查询时满足其一即可。一个Model class中允许指定多个SqlOrWhereAttribute实例。

Sets an optional search condition on top of the existing search condition in the model class. Either condition must be met. One or more SqlOrWhere attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlWhereAttribute](../SqlWhereAttribute/SqlWhereAttribute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlOrWhereAttribute : SqlWhereAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlOrWhereAttribute(string rawCondition)](Constructor/SqlOrWhereAttribute1.html) | Initializes a new instance of the SqlOrWhereAttribute class. |
| ![](~/images/method.jpeg) | [SqlOrWhereAttribute(string left, string right)](Constructor/SqlOrWhereAttribute2.html) | Initializes a new instance of the SqlOrWhereAttribute class. |

### **Remarks**

该特性必须同ModelAttribute.SqlWhereAttribute一同使用。

The SqlOrWhere attribute must be used together with ModelAttribute.SqlWhereAttribute.

SqlOrWhereAttribute 指明一个Model Class将在SQL SELECT语句中的WHERE Clause末尾添加OR logical operator and another search condition。

The SqlOrWhere attribute denotes that a model class should add an OR logical operator and another search  condition in the WHERE clause of the SQL SELECT statement.

### **Examples**



### **Applies to**

.NET Standard 

2.x