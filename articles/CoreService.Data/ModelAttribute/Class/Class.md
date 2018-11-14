## **Model Class Attributes**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png" class="dropdownpic"/></a>
<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>
<a href="javascript:void(0)">0.5.1-alpha(current)</a>
</div>
可作用于Model Class的特性的列表。

The list of attributes that can be applied to the model class.

**Namespace:** Appeon.CoreService.Data

**Assembly:** Appeon.CoreService.Data.dll



### **Properties**

|                                                              | Name                                                         | Description |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ----------- |
| ![](~/images/property.jpeg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | [DistinctAttribute](DistinctAttribute/DistinctAttribute.html) | Denotes that a model class should remove the duplicate values when loading data. |
| ![](~/images/property.jpeg) | [FromTableAttribute](FromTableAttribute/FromTableAttribute.html) | Specifies the database table that a model class is mapped to. Multiple FromTable attributes can be applied to one model class. |
| ![](~/images/property.jpeg) | [JoinTableAttribute](JoinTableAttribute/JoinTableAttribute.html) | Sets the joined table to be used in a model class. Multiple JoinTable attributes can be applied to one model class. |
| ![](~/images/property.jpeg) | [SqlAndHavingAttribute](SqlAndHavingAttribute/SqlAndHavingAttribute.html) | Sets an additional search condition on top of the existing search condition for a a group or an aggregate in the model class. Both conditions must be met. |
| ![](~/images/property.jpeg) | [SqlAndWhereAttribute](SqlAndWhereAttribute/SqlAndWhereAttribute.html) | Sets an additional search condition on top of the existing search condition in the model class. Both conditions must be met. |
| ![](~/images/property.jpeg) | [SqlGroupByAttribute](SqlGroupByAttribute/SqlGroupByAttribute.html) | Denotes that a model class should divide the query result into groups of rows. |
| ![](~/images/property.jpeg) | [SqlHavingAttribute](SqlHavingAttribute/SqlHavingAttribute.html) | Denotes that a model class should use a search condition for a group or an aggregate. |
| ![](~/images/property.jpeg) | [SqlOrderByAttribute](SqlOrderByAttribute/SqlOrderByAttribute.html) | Specifies how a model class sorts the result set when loading data. |
| ![](~/images/property.jpeg) | [SqlOrHavingAttribute](SqlOrHavingAttribute/SqlOrHavingAttribute.html) | Sets an optional search condition on top of the existing search condition for a group or an aggregate in the model class. Either condition must be met. |
| ![](~/images/property.jpeg) | [SqlOrWhereAttribute](SqlOrWhereAttribute/SqlOrWhereAttribute.html) | Sets an optional search condition on top of the existing search condition in the model class. Either condition must be met. |
| ![](~/images/property.jpeg) | [SqlParameterAttribute](SqlParameterAttribute/SqlParameterAttribute.html) | Defines a parameter with name and type in the model class. |
| ![](~/images/property.jpeg) | [SqlSelectAttribute](SqlSelectAttribute/SqlSelectAttribute.html) | Defines a select list in the model class, to decide which columns to be selected from the result set. The select list is a series of expressions separated by commas. |
| ![](~/images/property.jpeg) | [SqlUnionAttribute](SqlUnionAttribute/SqlUnionAttribute.html) | Denotes that a model class should combine the results of two or more queries into one single result. One or more SqlUnion attributes can be applied to one model class. |
| ![](~/images/property.jpeg) | [SqlWhereAttribute](SqlWhereAttribute/SqlWhereAttribute.html) | Sets the condition for the result set when a model class loads the data. |
| ![](~/images/property.jpeg) | [SubQueryAttribute](SubQueryAttribute/SubQueryAttribute.html) | Defines a subquery in the model class. |
| ![](~/images/property.jpeg) | [TopAttribute](TopAttribute/TopAttribute.html) | Denotes that a model class should limit the rows returned. |
| ![](~/images/property.jpeg) | [UpdateWhereStrategyAttribute](UpdateWhereStrategyAttribute/UpdateWhereStrategyAttribute.html) | Specifies the column(s) to be used as search condition when the model class is performing updates to the database. |

### **Remarks**















