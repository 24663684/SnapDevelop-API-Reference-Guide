

## **IDetailTracker.TrackDetailAndGrandDetail<TDetailModel, TGrandDetailModel>(Expression<Func<TModel, object>> propertyExpr, IModelEntry&#60;TDetailModel> modelEntry, Expression<Func<TDetailModel, object>> detailPropertyExpr, IModelEntry&#60;TGrandDetailModel> grandModelEntry) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

When working with three-level models which have master-detail-granddetail relationship by applying the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute in a property of the master model and a property of the detail model，追踪一个对detail model映射的数据库表的insert, update or delete操作,由数据的状态决定操作的类型，把即将被用来操纵数据库表的数据缓存于TDetailModel中,之后追踪一个对granddetail model映射的数据库表的insert, update or delete操作,由数据的状态决定操作的类型，把即将被用来操纵数据库表的数据缓存于TGrandDetailModel中。

当IModelMapper.SaveChanges被调用时，一条SQL INSERT, UPDATE or DELETE statement 将用缓存在TDetailModel中的数据以及被定义在TDetailModel中的映射信息来产生并执行，另外一条SQL INSERT, UPDATE or DELETE statement 将用缓存在TGrandDetailModel中的数据以及被定义在TGrandDetailModel中的映射信息来产生并执行。

Tracks an insert, update or delete operation on the table which the detail model is mapped to when working with the master-detail-granddetail models where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in a property of the master model and a property of the detail model. The data state determines which type of operation to be performed. The data to be manipulated is cached in TDetailModel. Then tracks an insert, update or delete operation on the table which the granddetail model is mapped to. The data state determines which type of operation to be performed. The data to be manipulated is cached in  TGrandDetailModel.

When IModelMapper.SaveChanges is called, two SQL statements (INSERT, UPDATE, or DELETE) will be generated, one is generated using the data cached in TDetailModel and the mapping information defined in TDetailModel, and the other is generated using the data cached in TGrandDetailModel and the mapping information defined in TGrandDetailModel; and then the two SQL statements will be executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  	IDetailTracker<TModel> TrackDetailAndGrandDetail<TDetailModel, TGrandDetailModel>(Expression<Func<TModel, object>> propertyExpr, IModelEntry<TDetailModel> modelEntry, Expression<Func<TDetailModel, object>> detailPropertyExpr, IModelEntry<TGrandDetailModel> grandModelEntry);

```

**Type Parameters**

`TDetailModel`

The type of a model class that conforms to the Appeon standard.

It is the type of the specified property in the detail model.

`TGrandDetailModel`

The type of a model class that conforms to the Appeon standard.

It is the type of the specified property in the granddetail model.

**Parameters**

`propertyExpr` System.Linq.Expressions.Expression<Func<TModel, object>>

主model的一个属性，其上实例化了ModelEmbeddedAttribute (ModelType属性是TDetailModel, 称为detail model)。

该属性的类型也是TDetailModel。

该属性由一个表达式指定。

A property of the master model where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute (the ModelType property is TDetailModel and is called detail model) is applied.

The type of this property is TDetailModel.

This property is specified by an expression.

`modelEntry` [Appeon.CoreService.Data.IModelEntry](../../IModelEntry/IModelEntry.html)&#60;TDetailModel>

需要跟踪的一个包装了数据和数据状态的IModelEntry对象.数据对应第一个属性表达式。

The IModelEntry object which packages the data and data state and which will be tracked. The data corresponds to the first property expression.

`detailPropertyExpr` System.Linq.Expressions.Expression<Func<TDetailModel, object>>

detail model的一个属性，其上实例化了ModelEmbeddedAttribute (ModelType属性是TGrandDetailModel, 称为granddetail model)。

该属性的类型是TGrandDetailModel。

该属性由一个表达式指定。

A property of the detail model where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute (the ModelType property is TGrandDetailModel and is called granddetail model) is applied.

The type of this property is TGrandDetailModel.

This property is specified by an expression.

`grandModelEntry` [Appeon.CoreService.Data.IModelEntry](../../IModelEntry/IModelEntry.html)&#60;TGrandDetailModel>

需要跟踪的一个包装了数据和数据状态的IModelEntry对象.数据对应第二个属性表达式。

The IModelEntry object which packages the data and data state and which will be tracked. The data corresponds to the second property expression.

**Returns**

Appeon.CoreService.Data.IDetailTracker&#60;TModel>

返回IDetailTracker&#60;TModel>接口对象。

Returns the IDetailTracker&#60;TModel> interface.

### **Remarks**

需要在TModel和TDetailModel 中定义ModelEmbedded attribute来表示TModel，TDetailModel和TGrandDetailModel的master-detail-granddetail relationship。

具体参考ModelEmbeddedAttribute中的相关说明。

The [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute must be applied in TModel and TDetailModel to create the master-detail-granddetail relationship between TModel, TDetailModel, and TGrandDetailModel. Refer to the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute for more.

#### One-to-one-to-one

propertyExpr参数指定的属性的类型是TDetailModel (该属性可代表数据库表的一行数据)，detailPropertyExpr参数指定的属性类型是TGrandDetailModel (该属性可代表数据库表的一行数据), 因此IDetailTracker.TrackDetailAndGrandDetail 方法适用于一行主表对应一行明细表再对应一行GrandDetail表的数据库表关系。

The type of the property specified by propertyExpr parameter is TDetailModel (which represents one row in the detail database table). The type of the property specified by detailPropertyExpr parameter is TGrandDetailModel (which represents one row in the granddetail database table). Therefore, the IDetailTracker.TrackDetailAndGrandDetail method applies to one-to-one-to-one table relationship (one master table record to one detail table record to one granddetail table record).

#### TrackMaster

IModelMapper.TrackMaster方法会在中跟踪master model之后会返回IDetailTracker接口对象。之后可以使用IDetailTracker.TrackDetailAndGrandDetail方法跟踪detail model和granddetail model。

The IModelMapper.TrackMaster method will track the master model and return the IDetailTracker interface. Then the IDetailTracker.TrackDetailAndGrandDetail method can be used to track the detail model and the granddetail model.

For more about the TrackMaster method, refer to IModelMapper.TrackMaster.

### **Examples**





### **Applies to**

.NET Standard 

2.x