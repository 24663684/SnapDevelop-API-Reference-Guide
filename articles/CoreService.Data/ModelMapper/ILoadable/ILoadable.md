## **ILoadable&#60;TModel> Interface**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
ILoadable接口提供了一系列用于数据加载后对数据进行操作的方法。

The ILoadable interface provides a series of methods for manipulating the data after loaded.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
 public interface ILoadable<TModel>;
```

### 

### **Methods**
|                                                      | Name    |Return type| Description                       |
| ---------------------------------------------------- |---------| ----------- | ------------------------------------- |
|![](~/images/method.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|[FirstOrDefault()](Method/FirstOrDefault.html)|TModel|Returns the first data record in the result set. If there is no data in the result set, returns the default value.|
| ![](~/images/method.jpeg)|[Include(Expression<Func<TModel, object>> property, bool cascade = false)](Method/Include1.html)|ILoadable&#60;TModel>|Loads data for the specified embedded property in TModel for all rows.|
| ![](~/images/method.jpeg)|[Include(int index, Expression<Func<TModel, object>> property, bool cascade = false)](Method/Include2.html)|ILoadable&#60;TModel>|Loads data for the specified embedded property in TModel for the specified row.|
| ![](~/images/method.jpeg)|[IncludeAll(bool cascade = false)](Method/IncludeAll1.html)|ILoadable&#60;TModel>|Loads data for the embedded properties in TModel for all rows.|
| ![](~/images/method.jpeg)|[IncludeAll(int index, bool cascade = false)](Method/IncludeAll2.html)|ILoadable&#60;TModel>|Loads data for the embedded properties in TModel for the specified row.|
| ![](~/images/method.jpeg)|[Load(params object[] parameters)](Method/Load1.html)|ILoadable&#60;TModel>|Retrieves data according to the SQL query defined in a TModel class.|
| ![](~/images/method.jpeg)|[Load(ISqlQueryBuilder queryBuilder, params object[] parameters);](Method/Load2.html)|ILoadable&#60;TModel>|Retrieves data according to the SQL query defined in the SqlQueryBuilder instance.|
| ![](~/images/method.jpeg)|[LoadByKey(params object[] parameters)](Method/LoadByKey.html)|ILoadable&#60;TModel>|Retrieves data according to the primary key defined in a TModel class.|
| ![](~/images/method.jpeg)|[ToArray()](Method/ToArray.html)|TModel|Converts the result set to a new array.|
| ![](~/images/method.jpeg)|[ToDictionary&#60;TKey>(Func<TModel, TKey> keySelector)](Method/ToDictionary.html)|Dictionary<TKey, TModel>|Creates a Dictionary<Tkey, TModel> from the result set according to the specified key selector function.|
| ![](~/images/method.jpeg)|[ToList()](Method/ToList.html)|List&#60;TModel>|Creates a List<TModel> from the result set.|
### **Remarks**

| Remarks                                                      |
| ------------------------------------------------------------ |
| IModelMapper接口的Load，LoadByKey方法会返回ILoadable接口对象，可以使用ILoadable提供的方法对数据进行操作, 比如使用ToList方法把数据转换为一个列表或者使用Include等方法对嵌入的Model进行操作。The IModelMapper.Load and IModelMapper.LoadByKey methods can return the ILoadable interface whose methods can be used to manipulate the data, for example, the ILoadable.ToList method can be used to convert the data to a list; the ILoadable.Include method can be used to manipulate the data in the embedded model. |

### **Examples**












