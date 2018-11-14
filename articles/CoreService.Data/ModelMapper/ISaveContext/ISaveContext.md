## **ISaveContext Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
一个可以访问或者操作保存数据过程中的上下文数据的接口。

This interface provides a series of methods for reading or manipulating the data context when saving the data changes to the database.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll



### **Syntax**

```c#
  public interface ISaveContext;
```


### **Properties**

|                             | Name                                     | Returns Type | Description |
| --------------------------- | ---------------------------------------- | -------- | ---- |
| ![](~/images/property.jpeg) | [Count](Property/Count.html) | int | Gets the number of the added values in the context of saving the data. |
| ![](~/images/property.jpeg) | [LastDbResult](Property/LastDbResult.html) | [IDbResult](../IDbResult/IDbResult.html) | Gets the result of the most recent operation that uses the model to save data to the database. |
| ![](~/images/property.jpeg) | [Names](Property/Names.html) | IReadOnlyList&#60;string> | Gets the name of all of the added values. |

### **Methods**

|                                                              | Name                                              | Returns Type | Description |
| ------------------------------------------------------------ | ------------------------------------------------- | ----------- | ----------- |
| ![](~/images/method.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | [Add(string name, object value)](Method/Add.html) | void        | Adds a value of any data type and its name to the save context. |
| ![](~/images/method.jpeg)                                    | [CancelSave()](Method/CancelSave.html)            | void        | Cancels the operation that is currently being executed to save the data to the database. |
| ![](~/images/method.jpeg)                                    | [Contains(string name)](Method/Contains.html)     | bool        | Returns whether the save context contains the specified value. |
| ![](~/images/method.jpeg)                                    | [Get(string name)](Method/Get.html)               | object      | Gets the specified value from the save context. |
| ![](~/images/method.jpeg)                                    | [Remove(string name)](Method/Remove.html)         | void        | Removes the specified value from the save context. |
| ![](~/images/method.jpeg)                                    | [RemoveAll()](Method/RemoveAll.html)              | void        | Removes all of the added values from the save context. |

### **Remarks**

| 说明 |
| ---- |
|      |

### **Examples**

















