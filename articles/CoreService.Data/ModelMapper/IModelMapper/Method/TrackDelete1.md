

## **IModelMapper.TrackDelete&#60;TModel>(TModel model) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表删除操作,将从数据库表删除的数据缓存于TModel中。当IModelMapper.SaveChanges被调用时，一条SQL DELETE statement 将用缓存在TModel中的数据以及被定义在TModel中的映射信息来产生，并执行。

Tracks a database table delete operation. The data that will be deleted from the database table is cached in TModel. When IModelMapper.SaveChanges is called, a SQL DELETE statement will be first generated using the data cached in TModel and the mapping information defined in TModel, and then executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackDelete<TModel>(TModel model);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`model` TModel

与数据库记录对应的TModel实例。

The TModel instance that corresponds to the database record.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x