## **SaveStrategy Enumeration**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
定义model class中的属性保存到数据库的可选策略。

Defines the optional strategies for the property to save data to the database.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public enum SaveStrategy
```

### **Members**

| Member name                                     | Description |
| ------------------------ | ----------------------------------------------------- |
| Save | 新增或者修改数据时保存 (Default)。Saves data to the database when data is inserted or updated  (Default). |
| SaveOnCreate | 仅插入数据时保存该属性的值到数据库。Saves data to the database when data is inserted. |
| SaveOnUpdate | 仅修改数据时保存该属性的值到数据库。Saves data to the database when data is updated. |
| ReadAfterSave | 保存数据记录后，从将数据库产生的值设置到该属性。Reads data for the property after data is saved to the database. |
| Ignore | 不保存到数据库。Not to save data to the database. |



### **Examples**















