## **SetValueStrategy Enumeration**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
用于SetValueAttribute中，指定需要设置值的时机。

Specifies the timing for the SetValue attribute to set values.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public enum SetValueStrategy
```

### **Member**

| Member Name                                    | Description |
| ------------------------ | ----------------------------------------------------- |
| Always | 在当前Model Class新增或者修改后，都对embedded Model Class中的指定属性设置值。Sets the value for the specified property in the embedded model class when data is inserted or updated in the current model class. |
| AfterParentCreated | 在当前Model Class新增后，对embedded Model Class中的指定属性设置值。Sets the value for the specified property in the embedded model class when data is inserted in the current model class. |
| AfterParentUpdated | 在当前Model Class修改后，对embedded Model Class中的指定属性设置值。Sets the value for the specified property in the embedded model class when data is updated in the current model class. |



### **Examples**















