## **SetValueAttribute.SetValueAttribute(string source, string target,  ModelSelector modelSelector) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SetValueAttribute class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
        public SetValueAttribute(string source, string target, SetValueStrategy setValueStrategy,ModelSelector modelSelector) 
```

**Parameters**

`source`	System.String

表示本级Model Class中的某个Properties。

A property of the model class at the same level.

格式:$PropertyName, 如:$Id。

Use this format to make reference: $PropertyName, for example, $Id.

`target` System.String

表示下一级Model Class中的某个Properties。

A property of the model class at one level lower.

格式:$PropertyName, 如:$Id
Use this format to make reference: $PropertyName, for example, $Id.

`setValueStrategy` [Appeon.CoreService.Data.SetValueStrategy](../../../SetValueStrategy/SetValueStrategy.html)

指定需要设置值的时机，是在本机Model Class新增后还是修改后。

The timing when the value needs to be set. Whether it is after the insert operation or the update operation in the model class at the same level.

默认为SetValueStrategy.Always表示在本级Model Class新增或者修改后，都对下一级的Model Class中的指定Properties设置值。

The default is SetValueStrategy.Always which indicates values should always be set for the specified property in the embedded model whenever there is an insert or update operation in the model at the same level.

`modelSelector` [Appeon.CoreService.Data.ModelSelector](../../../ModelSelector/ModelSelector.html)

根据下一级Model Class的实例的数据的状态来控制是否需要设置值。

Determines whether to set the value by the data state in the embedded model. 

默认为ModelSelector.All表示在下一级Model Class的实例无论是否已改变过数据都需要设置值。

The default is ModelSelector.All which indicates values should be set no matter the data has been updated or not in the embedded model.

### **Remarks**



### **Applies to**

.NET Standard 

2.x