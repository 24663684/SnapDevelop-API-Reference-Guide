## **SqlEmbeddedAttribute.ParamValue Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

获取或者设置加载当前Property的数据时需要传入的参数值。

Gets or sets the value of the parameter that is required when loading the data for the current property.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
    public string ParamValue { get; set; }
```

**Property Value**

System.String

一个表示加载当前Property的数据时需要传入的参数值的列表，与raw SQL SELECT Statement中定义的检索所需的参数一致。

A list of the parameter values that need to be passed in when loading the data for the current property. It has the same parameters required by the data retrieval in the raw SQL SELECT statement.

可以使用$加Master Model class的Property Name对Master Model中的一个值进行引用, 如$Id;

Use the $ symbol at the beginning of the property name of the master model class to make reference to value in the master model, for example, $Id.

也可以使用:加Master Model class中已定义的检索参数(使用SqlParameterAttribute)的Name对Master Model中的一个参数值进行引用, 如:param1;

You can also use the : symbol at the beginning of the name of the retrieval parameter (applying the SqlParameter attribute) of the master model class to make reference to a parameter value in the master model, for example, :param1.

当需要使用多个参数值时用逗号分割。如:$Id,:param1。

When there are multiple values, separate them with commas, for example, :$Id,:param1.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x