## **IEmbeddedLoadable.MasterModel Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Get a reference to the master model instance which is an argument when the IModelMapper.TrackMaster method is called. 

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   TModel MasterModel { get; }
```

**Returns**

System.TModel

A reference to the master model instance. 

### **Remarks**

The master model indicates the topmost-level model in the master-detail relationships created by applying the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute.

### **Examples**




### **Applies to**

.NET Standard 

2.x