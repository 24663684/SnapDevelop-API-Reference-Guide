## **ModelSelector Enumeration**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
用于SetValueAttribute,根据embedded Model Class的实例的数据修改状态来决定是否需要设置值。

The data state of the embedded model class that will be used by the SetValue attribute to determine whether to set values.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public enum ModelSelector
```

### **Members**

| Member Name                                     | Description |
| ------------------------ | ----------------------------------------------------- |
| All | All |
| ChangedOnly | 已修改的Changed data. |
| UnchangedOnly | 未修改的Unchanged data. |



### **Examples**















