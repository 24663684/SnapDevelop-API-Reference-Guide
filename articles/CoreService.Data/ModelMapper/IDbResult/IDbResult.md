## **IDbResult Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
一个用于访问保存数据到数据库的结果的interface.

This interface provides a series of properties for getting the result of saving the data changes to the database.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll


### **Syntax**

``` c#
  public interface IDbResult;
```

### **Properties**
|    | Name     |Return Type| Description     |
| -- |---|-----| ------ |
|![](~/images/property.jpeg)|[AffectedCount](Property/AffectedCount.html)|int|Gets the amount of rows that are affected when saving the data changes to the database.|
|![](~/images/property.jpeg)|[Cancelled](Property/Cancelled.html)|bool|Gets whether the operation is cancelled when saving the data changes to the database.|
|![](~/images/property.jpeg)|[DeletedCount](Property/DeletedCount.html)|int|Gets the amount of rows that are deleted when saving the data changes to the database.|
|![](~/images/property.jpeg)|[InsertedCount](Property/InsertedCount.html)|int|Gets the amount of rows that are inserted when saving the data changes to the database.|
|![](~/images/property.jpeg)|[ModifiedCount](Property/ModifiedCount.html)|int|Gets the amount of rows that are modified when saving the data changes to the database.|


### **Remarks**

| 说明 |
| ---- |
|      |




### **Examples**










