## **IDetailTracker&#60;TModel> Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
This interface provides a way to track data for detail models after the IModelMapper.TrackMaster method is called.

It is used when working with the master-detail models where the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute is applied in a property of the master model.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll


### **Syntax**

``` c#
  public interface IDetailTracker<TModel>;
```

### **Properties**
|    | Name     |Return Type| Description     |
| -- |---|-----| ------ |
|![](~/images/property.jpeg)|[MasterModel](Property/MasterModel.html)|TModel|Gets a reference to an internal TModel instance where the data is cached when the IModelMapper.TrackMaster method is called.|

### **Methods**
|  | Name    |Return Type| Description  |
| -- |----| --- | -------- |
|![](~/images/method.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|[SaveChanges(bool batchExecute = false)](Method/SaveChanges.html)|[IDbResult](../IDbResult/IDbResult.html)|Updates the database by executing the data changes tracked by a ModelMapper instance.|
|![](~/images/method.jpeg)|[TrackDetail&#60;TDetailModel>(Expression<Func<TModel, object>> propertyExpr, IModelEntry&#60;TDetailModel> modelEntry)](Method/TrackDetail.html)|[IDetailTracker&#60;TModel>](../IDetailTracker/IDetailTracker.html)|Tracks an operation on the detail table for the master-detail models.|
|![](~/images/method.jpeg)|[TrackDetailAndGrandDetail<TDetailModel, TGrandDetailModel>(Expression<Func<TModel, object>> propertyExpr, IModelEntry&#60;TDetailModel> modelEntry, Expression<Func<TDetailModel, object>> detailPropertyExpr, IModelEntry&#60;TGrandDetailModel> grandModelEntry)](Method/TrackDetailAndGrandDetail.html)|[IDetailTracker&#60;TModel>](../IDetailTracker/IDetailTracker.html)|Tracks an operation on the detail table and on the granddetail table for the master-detail-granddetail models.|
|![](~/images/method.jpeg)|[TrackDetailAndGrandDetails<TDetailModel, TGrandDetailModel>(Expression<Func<TModel, object>> propertyExpr, IModelEntry&#60;TDetailModel> modelEntry, Expression<Func<TDetailModel, object>> detailPropertyExpr, IEnumerable<IModelEntry&#60;TGrandDetailModel>> grandModelEntries)](Method/TrackDetailAndGrandDetails.html)|[IDetailTracker&#60;TModel>](../IDetailTracker/IDetailTracker.html)|Tracks an operation on the detail table and one or more operations on the granddetail table for the master-detail-granddetail models.|
|![](~/images/method.jpeg)|[TrackDetails&#60;TDetailModel>(Expression<Func<TModel, object>> propertyExpr, IEnumerable<IModelEntry&#60;TDetailModel>> modelEntry)](Method/TrackDetails.html)|[IDetailTracker&#60;TModel>](../IDetailTracker/IDetailTracker.html)|Tracks one or more operations on the detail table for the master-detail models.|


### **Remarks**

| Remarks                                                         |
| ------------------------------------------------------------ |
| IDetailTracker接口提供的方法和IModelMapper.TrackMaster方法一同使用，可以方便地在master-detail或者master-detail-granddetail这样的复杂的多层model关系下对数据进行追踪和保存。 IDetailTracker接口目前最多支持到三层model主从关系。The IDetailTracker interface provides a series of methods which when  used together with the IModelMapper.TrackMaster method can easily track and save data in the models with complex multi-level relationship such as master-detail or master-detail-granddetail. The IDetailTracker interface currently supports up to three levels of master-detail relationships. |




### **Examples**

待定。










