## **SetValueAttribute.SetValueAttribute( string source,string target) Constructor**

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
       public SetValueAttribute(string source,string target): this(source, target, SetValueStrategy.Always, ModelSelector.All)
```

**Parameters**

`source` System.String

表示本级Model Class中的某个Properties。

A property of the model class at the same level.

格式:$PropertyName, 如:$Id。

Use this format to make reference: $PropertyName, for example, $Id.

`target` System.String

表示下一级Model Class中的某个Properties。
A property of the model class at one level lower.

格式:$PropertyName, 如:$Id。

Use this format to make reference: $PropertyName, for example, $Id.

### **Remarks**



### **Applies to**

.NET Standard 

2.x