## **SetValueAttribute.Target Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取一个表示下一级Model Class中的某个Properties的string. 

Gets the string that represents a property in the model class at one level lower.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public string Target { get; }  
```

**Property Value**

System.String

表示下一级Model Class中的某个Properties。

The string that represents a property in the model class at one level lower.

格式:$PropertyName, 如:$Id

Use this format to make reference: $PropertyName, for example, $Id.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x