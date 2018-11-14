

## **ILoadable.ToDictionary&#60;TKey>(Func<TModel, TKey> keySelector) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

按照指定的key selector function从数据集中创建一个Dictionary<Tkey, TModel>。

Creates a Dictionary<Tkey, TModel> from the result set according to the specified key selector function.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  Dictionary<TKey, TModel> ToDictionary<TKey>(Func<TModel, TKey> keySelector);
```

**Parameters**

`keySelector` System.Func<TModel, TKey>

用于指定Dictionary key的function。

A function used to specify the Dictionary key.

**Returns**

System.Collections.Generic.Dictionary<TKey, TModel>

返回一个包含了数据集的所有数据的Dictionary<TKey, TModel>。

Returns an Dictionary<TKey, TModel> that includes all of the data of the result set.

### **Examples**





### **Applies to**

.NET Standard 

2.x