
# Application.OutlineShowTasks Method (Project)

Expands an outline to show all tasks up to the specified level and collapses any levels below.


## Syntax

 _expression_. **OutlineShowTasks**( **_OutlineNumber_**,  **_ExpandInsertedProjects_**)

 _expression_A variable that represents an  **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
|OutlineNumber|Optional| **Long**|The outline level to display. Higher outline levels are expanded to show this level. The level specified with  **OutlineNumber** and lower (if any) are collapsed. Can be one of the **[PjTaskOutlineShowLevel](27b015dd-5983-ca49-1a5d-67d71bb3d91f.md)** constants.|
|ExpandInsertedProjects|Optional| **Boolean**| **True** if tasks from subprojects are affected by the value specified with **OutlineNumber**. The default value is  **False**.|

### Return Value

 **Boolean**


## Example

This example has the same effect as collapsing the entire outline, including any tasks from subprojects.


```
Sub CollapseOutline() 
 Application.OutlineShowTasks pjTaskOutlineShowLevel1, True 
End Sub
```

