## **SqlUnionAttribute.UnionAll Property**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Gets or sets whether to use UNION ALL.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
    public bool UnionAll { get; set; }
```

**Property Value**

System.Boolean

True: use UNION ALL to incorporate all rows into the result (duplicates are included).

False: use UNION to incorporate all rows into the result (duplicates are removed).

The default is false.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x