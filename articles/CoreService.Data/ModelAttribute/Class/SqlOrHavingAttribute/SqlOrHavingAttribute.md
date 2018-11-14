## **SqlOrHavingAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

在一个Model Class中已有的search condition for a group or an aggregate的基础上，指定另外一个search condition，查询时满足其一即可。一个Model class中允许指定多个SqlOrHavingAttribute 实例。

Sets an optional search condition on top of the existing search condition for a group or an aggregate in the model class. Either condition must be met. One or more SqlOrHaving attributes can be applied to one model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlHavingAttribute](../SqlHavingAttribute/SqlHavingAttribute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct, AllowMultiple = true)]
   public class SqlOrHavingAttribute : SqlHavingAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                         |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](~/images/method.jpeg) | [SqlOrHavingAttribute(string rawCondition)](Constructor/SqlOrHavingAttribute1.html) | Initializes a new instance of the SqlOrHavingAttribute class. |
| ![](~/images/method.jpeg) | [SqlOrHavingAttribute(string left, string right)](Constructor/SqlOrHavingAttribute2.html) | Initializes a new instance of the SqlOrHavingAttribute class. |

### **Remarks**

该特性必须同ModelAttribute.SqlHavingAttribute一同使用。

The SqlOrHaving attribute must be used together with ModelAttribute.SqlHavingAttribute.

SqlOrHavingAttribute 指明一个Model Class将在SQL SELECT语句中的HAVING Clause中添加OR logical operator and another search condition。

The SqlOrHaving attribute denotes that a model class should add an OR logical operator and another search condition in the HAVING clause of the SQL SELECT statement.

### **Examples**



### **Applies to**

.NET Standard 

2.x