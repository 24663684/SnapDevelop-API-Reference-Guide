

## **IDetailTracker.TrackDetails&#60;TDetailModel>(Expression<Func<TModel, object>> propertyExpr, IEnumerable<IModelEntry&#60;TDetailModel>> modelEntry) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

When working with multiple models which have Master-Detail relationship by instantiating ModelEmbedded attribute in a property of the master model，追踪一个或者多个对detail model映射的数据库表的insert, update or delete操作,由数据的状态决定操作的类型，把即将被用来操纵数据库表的数据缓存于TDetailModel中。

当IModelMapper.SaveChanges被调用时，一条或者多条SQL INSERT, UPDATE or DELETE statement 将用缓存在TDetailModel中的数据以及被定义在TDetailModel中的映射信息来产生并执行。

Tracks one or more insert, update or delete operations on the table which the detail model is mapped to, when working with the master-detail models (where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in a property of the master model). The data state determines which type of operation to be performed. The data to be manipulated is cached in TDetailModel.

When IModelMapper.SaveChanges is called, one ore more SQL statements (INSERT, UPDATE, or DELETE) will be first generated using the data cached in TDetailModel and the mapping information defined in TDetailModel, and then executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  IDetailTracker<TModel> TrackDetails<TDetailModel>(Expression<Func<TModel, object>> propertyExpr, IEnumerable<IModelEntry<TDetailModel>> modelEntry);
```

**Type Parameters**

`TDetailModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`propertyExpr` System.Linq.Expressions.Expression<Func<TModel, object>>

主model的一个属性，其上实例化了ModelEmbeddedAttribute (ModelType属性是TDetailModel, 称为detail model)。

该属性的类型是a collection of TDetailModel。

该属性由一个表达式指定。

A property of the master model where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute (the ModelType property is TDetailModel and is called detail model) is applied.

The type of this property is a collection of TDetailModel.

This property is specified by an expression.

`modelEntry` System.Collections.Generic.IEnumerable<[Appeon.CoreService.Data.IModelEntry](../../IModelEntry/IModelEntry.html)&#60;TDetailModel>>

需要跟踪的一个包装了数据和数据状态的IModelEntry对象的集合。

The collection of IModelEntry object which packages the data and data state and which will be tracked.

**Returns**

Appeon.CoreService.Data.IDetailTracker&#60;TModel>

返回IDetailTracker&#60;TModel>接口对象。

Returns the IDetailTracker&#60;TModel> interface.

### **Remarks**

需要在TModel中定义ModelEmbedded attribute来表示TModel和TDetailModel的Master-Detail relationship，具体参考ModelEmbeddedAttribute中的相关说明。

The [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute must be applied in TModel to create the master-detail relationship between TModel and TDetailModel. Refer to the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute for more.

#### One-to-many

propertyExpr参数指定的属性的类型是a collection of TDetailModel (该属性可代表数据库表的多行数据)，IDetailTracker.TrackDetails方法适用于一行主表对应多行明细表的数据库表关系。

如需使用一行主表对多行明细表的关系，可以使用IDetailTracker.TrackDetails替代。

The type of the property specified by propertyExpr parameter is a collection of TDetailModel (which represents one or more records in the detail table). The IDetailTracker.TrackDetails method applies to the one-to-many table relationship (one master table record to many detail table records).

For one-to-one relationship (one master table record to one detail table record), uses IDetailTracker.TrackDetail method instead.

#### TrackMaster

IModelMapper.TrackMaster方法会在中跟踪master model之后会返回IDetailTracker接口对象。之后可以使用IDetailTracker.TrackDetail方法跟踪detail model。

The IModelMapper.TrackMaster method will track the master model and return the IDetailTracker interface. Then the IDetailTracker.TrackDetail method can be used to track the detail model.

For more about the TrackMaster method, refer to IModelMapper.TrackMaster.

### **Examples**





### **Applies to**

.NET Standard 

2.x