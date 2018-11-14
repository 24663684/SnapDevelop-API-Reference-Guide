## **IModelEntry Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
一个可以对含有数据和状态的ModelEntry object进行访问或者操作的接口。

This interface provides methods, properties, and events for accessing and manipulating internal ModelEntry object which contains data and state.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public interface IModelEntry;
```

### **事件**

|                          | Name                                                  | Description                               |
| ------------------------ | ----------------------------------------------------- | ----------------------------------------- |
| ![](~/images/event.jpeg) | [CurrentValueChanged](Event/CurrentValueChanged.html) | Occurs when the current value is changed. |


### ** Property**

|                             | Name                                     | Returns Type | Description |
| --------------------------- | ---------------------------------------- | -------- | ---- |
| ![](~/images/property.jpeg) | [ModelState](Property/ModelState.html)   | [ModelState](../ModelState/ModelState.html) | Gets the tracked state of the data. |
| ![](~/images/property.jpeg) | [Properties](Property/Properties.html)   | int      | Gets the property names of the model class. |

### **方法**

|                                                              | Name                                                         | Returns Type                                         | Description                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------------- | -------------------------------------------------- |
| ![](~/images/method.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | [GetPropertyState(string name)](Method/GetPropertyState.html) | [PropertyState](../PropertyState/PropertyState.html) | Gets the tracked state of the specified property.  |
| ![](~/images/method.jpeg)                                    | [GetOriginalValue(string name)](Method/GetOriginalValue.html) | object                                               | Gets the original value of the specified property. |
| ![](~/images/method.jpeg)                                    | [GetCurrentValue(string name)](Method/GetCurrentValue.html)  | object                                               | Gets the current value of the specified property.  |
| ![](~/images/method.jpeg)                                    | [SetCurrentValue(string name, object value)](Method/SetCurrentValue.html) | void                                                 | Sets the current value for the specified property. |

### **Remarks**

| 说明 |
| ---- |
|      |

### **Examples**















