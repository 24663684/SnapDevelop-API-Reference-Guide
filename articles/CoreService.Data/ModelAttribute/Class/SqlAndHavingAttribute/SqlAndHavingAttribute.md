## ** ModelAttribute.SqlAndHavingAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class中已有的search condition for a group or an aggregate的基础上，指定需要同时满足的另外一个search condition。一个Model class中允许指定多个SqlAndHavingAttribute 实例。

Sets an additional search condition on top of the existing search condition for a a group or an aggregate in the model class. Both conditions must be met. One or more SqlAndHaving attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlHavingAttribute](../SqlHavingAttribute/SqlHavingAttribute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlAndHavingAttribute : SqlHavingAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlAndHavingAttribute(string rawCondition)](Constructor/SqlAndHavingAttribute1.html) | Initializes a new instance of the SqlAndHavingAttribute class. |
| ![](~/images/method.jpeg) | [SqlAndHavingAttribute(string left, string right)](Constructor/SqlAndHavingAttribute2.html) | Initializes a new instance of the SqlAndHavingAttribute class. |

### **Remarks**

该特性必须同ModelAttribute.SqlHavingAttribute一同使用。

The SqlAndHaving attribute must be used together with ModelAttribute.SqlHavingAttribute.

SqlAndHavingAttribute 指明一个Model Class将在原有SQL SELECT语句中的HAVING Clause中添加AND logical operator and another search condition。

The SqlAndHaving attribute denotes that a model class should add an AND logical operator and another search condition in the HAVING clause of the SQL SELECT statement.

### **Examples**



### **Applies to**

.NET Standard 

2.x