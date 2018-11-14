

## **ILoadable.FirstOrDefault() Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

返回数据集的第一条数据，如果数据集中没有数据则返回默认值。Returns the first data record in the result set. If there is no data in the result set, returns the default value.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  TModel FirstOrDefault();
```

**Returns**

System.TModel

Returns a TModel type object which represents the first row of the result set loaded, or returns null if no rows loaded. 

### **Remarks**

IModelMapper.Load，IModelMapper.LoadByKey数据加载 Method返回ILoadable接口对象，可以利用ILoadable接口提供的 Method操作加载的数据，ILoadable.FirstOrDefault Method用于获取加载数据的第一条数据。

IModelMapper.Load and IModelMapper.LoadByKey methods return the ILoadable object whose methods can be used to manipulate the loaded data. The ILoadable.FirstOrDefault method is used to obtain the first data record that is loaded.

### **Examples**





### **Applies to**

.NET Standard 

2.x