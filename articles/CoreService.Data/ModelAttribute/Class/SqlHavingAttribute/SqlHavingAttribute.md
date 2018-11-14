## **SqlHavingAttribute Class**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指明一个Model Class将使用一个组或者聚合的搜索条件。

Denotes that a model class should use a search condition for a group or an aggregate.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Inheritance Constructor**

[Appeon.CoreService.Data.SqlWhereAttribute](../SqlWhereAttribute/SqlWhereAttribute.html)

### **Syntax**

```c#
   [AttributeUsage(AttributeTargets.Class | AttributeTargets.Struct)]
   public class SqlHavingAttribute : SqlWhereAttribute
```

### **Constructors**

|                           | Name                                                         | Description                                                        |
| ------------------------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| ![](~/images/method.jpeg) | [SqlHavingAttribute(string rawCondition)](Constructor/SqlHavingAttribute1.html) | Initializes a new instance of the SqlHavingAttribute class. |
| ![](~/images/method.jpeg) | [SqlHavingAttribute(string left, string right)](Constructor/SqlHavingAttribute2.html) | Initializes a new instance of the SqlHavingAttribute class. |



### **Remarks**

The SqlHaving attribute is typically used with the SqlGroupBy attribute.



SqlHavingAttribute指明一个Model Class将在SQL SELECT语句中使用HAVING Clause来定义一个组或者聚合的搜索条件。

The SqlHaving attribute denotes that a model class should use a HAVING clause in the SQL SELECT statement to define the search condition for a group or an aggregate.

### **Examples**



### **Applies to**

.NET Standard 

2.x