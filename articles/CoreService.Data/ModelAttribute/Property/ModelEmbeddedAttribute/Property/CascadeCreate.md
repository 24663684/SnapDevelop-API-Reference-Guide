## **ModelEmbeddedAttribute.CascadeCreate Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取或者设置当Model Class在新增数据时，是否自动级联新增当前Property中的数据。

Gets or sets whether to insert data to the associated property in the detail model or the granddetail model when the model class is inserting data.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public bool CascadeCreate { get; set; }
```

**Property Value**

System.Boolean

True, 当Model Class在新增数据时，自动级联新增当前Property中的数据。

True: insert data to the associated property in the detail model or the granddetail model when the model class is inserting data.

False, 当Model Class在新增数据时，不处理当前Properties。

False: not to insert data to the associated property in the detail model or the granddetail model when the model class is inserting data.

### **Remarks**

当IModelMapper的TrackCreate方法追踪Master Model对象的时，将同时追踪Master Model Class中所有指定了ModelEmbedded特性并且ModelEmbedded特性的CascadeCreate为True的Property中的数据。

When the IModelMapper TrackCreate method tracks the master model, it also tracks the data of properties in the master model class where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied and the CascadeCreate parameter of ModelEmbedded is set to true.

### **Examples**



### **Applies to**

.NET Standard 

2.x