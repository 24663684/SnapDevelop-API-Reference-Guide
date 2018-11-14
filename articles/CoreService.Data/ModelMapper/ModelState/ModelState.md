## **ModelState Enumeration**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>

Specifies the tracked state of the model instance.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll



### **Syntax**

```c#
   public enum ModelState;
```

### **Fields**

| Name                                                | Description |
| ------------------------ | ----------------------------------------------------- |
| NotTracked | This model has not been tracked. |
| NotModified | No data has been changed since retrieved. |
| Modified | Data has been changed since retrieved.                       |
| New | Data is newly added and no values have been specified for its properties. |
| NewModified | Data is newly added, and values have been assigned to its properties. |
| Deleted | Data has been deleted since retrieved. |



### **Examples**















