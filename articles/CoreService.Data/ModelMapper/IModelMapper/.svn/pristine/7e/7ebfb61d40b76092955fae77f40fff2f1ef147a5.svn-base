

## **IModelMapper.TrackUpdate&#60;TModel>(TModel model, Action&#60;ISaveContext> afterSaveAction) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表修改操作和一个Action Delegate,将在数据库表修改的数据缓存于TModel中。当IModelMapper.SaveChanges被调用时，一条SQL UPDATE statement 将用缓存在TModel中的数据以及被定义在TModel中的映射信息来产生，并执行，之后调用the Action Delegate。

Tracks a database table update operation and an Action delegate. The data that will be updated to the database table is cached in TModel. When IModelMapper.SaveChanges is called, a SQL UPDATE statement will be first generated using the data cached in TModel and the mapping information defined in TModel, and then executed, and after that, the Action delegate will be called.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackUpdate<TModel>(TModel model, Action<ISaveContext> afterSaveAction);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`model` System.TModel

一个与数据库记录对应的TModel实例。

The TModel instance that corresponds to the database record.

`afterSaveAction` System.Action[<Appeon.CoreService.Data.ISaveContext>](../../ISaveContext/ISaveContext.html)

一个需要追踪的Action Delegate。

An Action delegate that needs to be tracked.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**

在实例化Action Delegate时，可以使用ISaveContext泛型参数来读写保存数据过程中内部使用的上下文，具体请参考ISaveContext。

When instantiating the Action delegate, the generic parameter of ISaveContext can be used for reading and writing the context which is used internally for saving data. See ISaveContext for more info.

### **Examples**



### **Applies to**

.NET Standard 

2.x