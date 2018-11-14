## **ModelEmbeddedAttribute.QueryExpression Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

指定与当QuerySelectorProperties的查询方式相应的SQL Expression参数。

Sets the SQL expression parameter that corresponds to the query method of the QuerySelector property.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public string QueryExpression { get; set; }
```

**Property Value**

System.String

A SQL expression.

当QuerySelectorProperties被设置为QuerySelect.SelectCount等查询方式时则必须设置QueryExpressionProperties;

When the QuerySelector property is set to QuerySelect.SelectCount etc., the QueryExpression property must be set.

当QuerySelectorProperties被设置为QuerySelect.Select或者QuerySelect.SelectByKey的时候无需设置QueryExpressionProperties。

When the QuerySelector property is set to QuerySelect.Select or QuerySelect.SelectByKey, the QueryExpression property is not required to be set.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x