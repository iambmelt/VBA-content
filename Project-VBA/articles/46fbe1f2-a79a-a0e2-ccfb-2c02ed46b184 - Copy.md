
# Application.VisualReportsNewTemplate Method (Project)

Creates a Visual Reports template for Microsoft Excel or Microsoft Visio.


## Syntax

 _expression_. **VisualReportsNewTemplate**( **_PjVisualReportsTemplateType_**,  **_PjVisualReportsCubeType_**,  **_ReportAlLFields_**,  **_PjVisualReportsDataLevel_**)

 _expression_A variable that represents an  **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
|PjVisualReportsTemplateType|Optional| **Long**|Template type. Can be one of the  **[PjVisualReportsTemplateType](66c80c6d-434c-5983-45fb-48120db7a8b6.md)** constants. Default is **pjExcel**.|
|PjVisualReportsCubeType|Optional| **Long**|Cube type. Can be one of the  **[PjVisualReportsCubeType](dd05c192-8213-e6fc-0060-c32c761ec5d5.md)** constants. Default is **pjTaskTP**.|
|ReportAlLFields|Optional| **Boolean**|If  **True**, all noncustom fields are included in the report. |
|PjVisualReportsDataLevel|Optional| **Long**|Data level. Can be one of the  **[PjVisualReportsDataLevel](56792ea8-6459-38ef-e994-95024e6d8fe9.md)** constants. Default is **pjLevelAutomatic**.|

### Return Value

 **Boolean**


## Remarks

Setting the ReportAllFields parameter to  **True** can degrade performance.

The PjVisualReportsDataLevel parameter specifies the level to which the timephased data can be accessed. For example, if  **pjLevelMonths** (months) is specified, it not possible to access **pjLevelDays** (days).

