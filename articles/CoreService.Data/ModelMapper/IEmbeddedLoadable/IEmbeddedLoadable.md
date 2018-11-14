## **IEmbeddedLoadable&#60;TModel> Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
IEmbeddedLoadable接口提供了一系列用于对嵌入属性(实例化了ModelEmbeddedAttribute or SqlEmbeddedAttribute)的数据进行操作的方法。

The IEmbeddedLoadable interface provides a series of methods for manipulating the data in the embedded properties where either the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll


### **Syntax**

``` c#
  public interface IEmbeddedLoadable<TModel>;
```

### **Properties**
|    | Name     |Return type| Description     |
| -- |---|-----| ------ |
|![](~/images/property.jpeg)|[MasterModel](Property/MasterModel.html)|TModel|Get a reference to the master model instance which is an argument when the IModelMapper.TrackMaster method is called.|

### **Methods**
|  | Name    |Return type| Description  |
| -- |----| --- | -------- |
|![](~/images/method.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|[Include(Expression<Func<TModel, object>> property, bool cascade = false)](Method/Include.html)|[ILoadable&#60;TModel>](../ILoadable/ILoadable.html)|Loads data for the specified embedded property in TModel for all rows.|
|![](~/images/method.jpeg)|[IncludeAll(bool cascade = false)](Method/IncludeAll.html)|[ILoadable&#60;TModel>](../ILoadable/ILoadable.html)|Loads data for the embedded properties in TModel for all rows.|


### **Remarks**

| 说明                                                         |
| ------------------------------------------------------------ |
| IModelMapper.IModelMapper.LoadEmbedded方法会返回IEmbeddedLoadable接口对象，可以使用IEmbeddedLoadable提供的方法对数据进行操作, 比如使用Include等方法对嵌入的属性进行操作. The IModelMapper.LoadEmbedded method will return an IEmbeddedLoadable interface whose methods can be used to manipulate the data, for example, the Include method can be used to manipulate the data in the embedded properties where either the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute or the [SqlEmbedded](../../ModelAttribute/Property/SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) attribute is applied.<br/><br/>请参考IModelMapper.LoadEmbedded方法的更多信息. Refer to IModelMapper.LoadEmbedded for more info. |


### **Examples**










