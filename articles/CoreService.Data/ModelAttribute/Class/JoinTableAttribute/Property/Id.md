## **JoinTableAttribute.Id Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取在Model Class中的指定的joined table的唯一ID。

Gets the ID of the joined table in the model class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public int Id { get; internal set; }
```

**Property Value**

System.Int32

指定的joined table的唯一ID

ID of the joined table.

### **Remarks**

该ID可表示某个表(含被连接的表)在SQL SELECT Statement的FROM Clause中出现的次序。

ID can represent the order of a table (and the joined table) in the FROM clause of the SQL SELECT statement.

### **Examples**



### **Applies to**

.NET Standard 

2.x