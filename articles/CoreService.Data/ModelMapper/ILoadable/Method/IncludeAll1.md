

## **ILoadable.IncludeAll(bool cascade = false); Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Loads所有行的TModel中所有实例化了ModelEmbeddedAttribute 或者SqlEmbeddedAttribute属性的数据。

当该属性实例化了ModelEmbedded时，将根据ModelEmbedded的ModelType属性对应detail model中定义的 SQL query从数据库检索数据。可使用cascade参数是控制是否级联Load该detail model中实例化了ModelEmbeddedAttribute或者SqlEmbeddedAttribute的属性。

Loads data for the embedded properties (where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied) in TModel for all rows.

If the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in the property, the property will use the SQL query (defined in the detail model class specified by the ModelType property of the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute) to retrieve data from database. The cascade parameter can be used to decide whether to retrieve data for the embedded properties in the detail model or the granddetail model.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  ILoadable<TModel> IncludeAll(bool cascade = false);
```

**Parameters**

 `cascade` System.Boolean

Only when the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in the property, the cascade parameter can be used to decide whether to retrieve data for the embedded properties in the detail model or the granddetail model. 

The default value is false.

**Returns**

Appeon.CoreService.Data.ILoadable&#60;TModel>

Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**



### **Examples**





### **Applies to**

.NET Standard 

2.x