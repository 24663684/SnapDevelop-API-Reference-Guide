

## **IModelMapper.Track(Action&#60;ISaveContext> saveAction) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个Action delegate。当IModelMapper.SaveChanges被调用时，将调用这个Action delegate。
Tracks an Action delegate. The Action delegate will be called when IModelMapper.SaveChanges is called.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper Track(Action<ISaveContext> saveAction);
```

**Parameters**

`saveAction` System.Action<[Appeon.CoreService.Data.ISaveContext](../../ISaveContext/ISaveContext.html)>

一个需要追踪的Action Delegate。
An Action delegate that needs to be tracked. 

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。
Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**

在实例化Action Delegate时，可以使用ISaveContext的泛型参数来读写保存数据过程中内部使用的上下文，具体请参考ISaveContext。

When instantiating the Action delegate, the generic parameter of ISaveContext can be used for reading and writing the context which is used internally for saving data. See ISaveContext for more info.


当调用ModelMapper的多个追踪 Method后，追踪的先后顺序决定了实际执行数据库操作的先后顺序。

After calling multiple track methods of ModelMapper, the order of tracks determines the order of the actual operations to the database.


### **Examples**



### **Applies to**

.NET Standard 

2.x