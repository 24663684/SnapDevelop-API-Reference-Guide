## **Model Property Attributes**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
可作用于Model Class的Properties的特性的列表。

The list of attributes that can be applied to the property of a model class.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll



### **Properties**

|                                                              | Name                                                         | Description |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ----------- |
| ![](~/images/property.jpeg) | [IdentityAttribute](IdentityAttribute/IdentityAttribute.html) | Specifies that the database generates a value for the property when a row is inserted. |
| ![](~/images/property.jpeg) | [ModelEmbeddedAttribute](ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) | Specifies that a property in the model class will use the specified model class to load and update data independently. |
| ![](~/images/property.jpeg) | [NotInWhereAttribute](NotInWhereAttribute/NotInWhereAttribute.html) | This attribute takes no effect at this moment. |
| ![](~/images/property.jpeg) | [PropertySaveAttribute](PropertySaveAttribute/PropertySaveAttribute.html) | Specifies the strategy to be used when saving the data for a property to the database. |
| ![](~/images/property.jpeg) | [SetValueAttribute](SetValueAttribute/SetValueAttribute.html) | Specifies that when there is an insert or update operation in the master model, set the property value of the master model to the associate property of the detail model |
| ![](~/images/property.jpeg) | [SqlColumnAttribute](SqlColumnAttribute/SqlColumnAttribute.html) | Represents the database column that a property is mapped to. |
| ![](~/images/property.jpeg) | [SqlComputeAttribute](SqlComputeAttribute/SqlComputeAttribute.html) | Represents a computed column that a property is mapped to. |
| ![](~/images/property.jpeg) | [SqlEmbeddedAttribute](SqlEmbeddedAttribute/SqlEmbeddedAttribute.html) | Specifies that a property of the model class will use the specified raw SQL SELECT statement to load data. |
| ![](~/images/property.jpeg) | [SqlJoinAndOnAttribute](SqlJoinAndOnAttribute/SqlJoinAndOnAttribute.html) | Specifies the condition for joining a table, using the AND operator. |
| ![](~/images/property.jpeg) | [SqlJoinOnAttribute](SqlJoinOnAttribute/SqlJoinOnAttribute.html) | Specifies the condition for joining a table. |
| ![](~/images/property.jpeg) | [SqlJoinOrOnAttribute](SqlJoinOrOnAttribute/SqlJoinOrOnAttribute.html) | Specifies the condition for joining a table, using the OR operator. |

### **Remarks**















