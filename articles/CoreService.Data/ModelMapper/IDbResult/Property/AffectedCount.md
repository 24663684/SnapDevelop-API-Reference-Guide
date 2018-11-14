## **IDbResult.AffectedCount Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Get 保存数据到数据库时受影响的行数.

Gets the amount of rows that are affected when saving the data changes to the database.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   int InsertedCount { get; }
```

**Returns**

System.Int32

受影响的行数。等于InsertedCount,DeletedCount,和ModifiedCount三个属性之和。

The amount of rows that are affected. It is equivalent to a sum of InsertedCount, DeletedCount, and ModifiedCount properties.

### **Remarks**



### **Examples**





### **Applies to**

.NET Standard 

2.x