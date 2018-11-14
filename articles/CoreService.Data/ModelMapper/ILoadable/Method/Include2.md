

## **ILoadable.Include(int index, Expression<Func<TModel, object>> property, bool cascade = false) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Loads指定行的TModel中指定的实例化了ModelEmbeddedAttribute 或者SqlEmbeddedAttribute的属性的数据。

当该属性实例化了ModelEmbedded时，将根据ModelEmbedded的ModelType属性对应detail model中定义的 SQL query从数据库检索数据。可使用cascade参数是控制是否级联Load该detail model中实例化了ModelEmbeddedAttribute或者SqlEmbeddedAttribute的属性。

Loads data for the specified embedded property (where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied) in TModel for the specified row.

If the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in the property, the property will use the SQL query (defined in the detail model class specified by the ModelType property of the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute) to retrieve data from database. The cascade parameter can be used to decide whether to retrieve data for the embedded properties in the detail model or the granddetail model.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  ILoadable<TModel> Include(int index, Expression<Func<TModel, object>> property, bool cascade = false);
```

**Parameters**

 `index` System.Int32

数据集的行索引。

The zero-based index for the row in the result set.

`property` System.Linq.Expressions.Expression

TModel的一个需要load数据的属性，其上实例化了ModelEmbeddedAttribute或者SqlEmbeddedAttribute。

该属性由一个表达式指定。

A property of TModel where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied.

This property is specified by an expression.

`cascade` System.Boolean

Only when the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in the property, the cascade parameter can be used to decide whether to retrieve data for the embedded properties in the detail model or granddetail model. 

The default value is false.

**Returns**


Appeon.CoreService.Data.ILoadable&#60;TModel>


Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**

ILoadable.Include Method可以根据需要加载某行的一个实例化了ModelEmbedded或者SqlEmbedded特性的属性的数据，而不必把所有属性的数据都加载出来，这样有利于提升数据的查询效率。

The ILoadable.Include method can be used to load the data for the specified embedded property (where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied) for the specified row, rather than loading data for all of the properties. This can greatly improve the data retrieval efficiency.

### **Examples**





### **Applies to**

.NET Standard 

2.x