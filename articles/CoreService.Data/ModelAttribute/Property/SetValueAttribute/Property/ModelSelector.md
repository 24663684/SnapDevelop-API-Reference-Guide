## **SetValueAttribute.ModelSelector Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取已一个ModelSelector枚举项，该ModelSelector枚举项将根据下一级Model Class的实例的数据修改状态来决定是否需要设置值。

Gets the ModelSelector enumerated value which determines whether to set value by the data state in the embedded model.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public ModelSelector ModelSelector { get; }
```

**Property Value**

[Appeon.CoreService.Data.ModelSelector](../../../../ModelSelector/ModelSelector.html)

根据下一级Model Class的实例的数据修改状态来决定是否需要设置值。

Determines whether to set the value by the data state in the embedded model. 

默认为ModelSelector.All，表示在下一级Model Class的实例无论是否已改变过数据都需要设置值。

The default is ModelSelector.All which indicates values should be set no matter the data has been updated or not in the embedded model.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x