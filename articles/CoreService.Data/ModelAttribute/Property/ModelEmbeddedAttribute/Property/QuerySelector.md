## **ModelEmbeddedAttribute.QuerySelector Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取或者设置当前Property在加载数据时使用怎样的查询方式。

Gets or sets the query method to be used when loading the data for the current property.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public QuerySelector QuerySelector { get; set; }
```

**Property Value**

[Appeon.CoreService.Data.QuerySelector](../../../../QuerySelector/QuerySelector.html)

当前Property在加载数据时使用的查询方式，默认使用QuerySelector.Select.

The query method to be used when loading the data for the current property. By default, QuerySelector.Select is used.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x