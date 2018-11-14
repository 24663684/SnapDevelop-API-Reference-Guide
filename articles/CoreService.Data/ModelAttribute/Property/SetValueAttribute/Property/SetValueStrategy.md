## **SetValueAttribute.SetValueStrategy Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取一个SetValueStrategy枚举项，它指定需要设置值的时机。

Gets the SetValueStrategy enumerated value which determines when to set value.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public SetValueStrategy SetValueStrategy { get; }
```

**Property Value**

[Appeon.CoreService.Data.SetValueStrategy](../../../../SetValueStrategy/SetValueStrategy.html)

指定需要设置值的时机。

Timing to set value.

默认为SetValueStrategy.Always表示在本级Model Class新增或者修改后，都对下一级的Model Class中的指定Properties设置值。

The default is SetValueStrategy.Always which indicates values should always be set for the specified property in the embedded model whenever there is an insert or update operation in the model at the same level.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x