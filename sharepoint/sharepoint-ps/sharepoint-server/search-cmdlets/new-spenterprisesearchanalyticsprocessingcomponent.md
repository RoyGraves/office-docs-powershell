---
title: "New-SPEnterpriseSearchAnalyticsProcessingComponent"
ms.author: tlarsen
author: tlarsen
manager: laurawi
ms.date: 11/29/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c659be08-f187-4ab1-b841-205e8316218b

description: "Creates a new analytics processing component for the given topology and search service instance."
---

# New-SPEnterpriseSearchAnalyticsProcessingComponent

Creates a new analytics processing component for the given topology and search service instance.
  
```
New-SPEnterpriseSearchAnalyticsProcessingComponent -SearchServiceInstance <SearchServiceInstancePipeBind> -SearchTopology <SearchTopologyPipeBind> [-AssignmentCollection <SPAssignmentCollection>] [-Confirm [<SwitchParameter>]] [-SearchApplication <SearchServiceApplicationPipeBind>] [-WhatIf [<SwitchParameter>]]

```

## Example

------------------EXAMPLE-----------------
  
```
$ssa = Get-SPEnterpriseSearchServiceApplication

```

```
New-SPEnterpriseSearchAnalyticsProcessingComponent -SearchTopology 06e6651d-ecdd-4105-bb65-6a83b6155525 -SearchServiceInstance 56e6651d-ecdd-4105-bb65-6a83b6155525 -SearchApplication $ssa
```

This example adds a new analytics processing component to the search topology with identity  `06e6651d-ecdd-4105-bb65-6a83b6155525` in the search service instance with identity  `56e6651d-ecdd-4105-bb65-6a83b6155525` in the default search service application referenced by  `$ssa`.
  
## Detailed Description

Creates a new analytics processing component and adds it to an inactive search topology in a specific search service instance. The change is effectuated when the search topology is enabled.
  
For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at [Windows PowerShell for SharePoint Server 2016 reference](https://go.microsoft.com/fwlink/p/?LinkId=671715). 
  
## Parameters

|**Parameter**|**Required**|**Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _SearchServiceInstance_ <br/> |Required  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchServiceInstancePipeBind  <br/> |Specifies the search service instance that will host the new analytics processing component. The type must be a valid GUID, in the form 12345678-90ab-cdef-1234-567890bcdefgh, a valid name of a search topology server, or an instance of a valid **SearchServiceInstance** object.  <br/> |
| _SearchTopology_ <br/> |Required  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchTopologyPipeBind  <br/> |Specifies the search topology where the new analytics processing component should be added.  <br/> |
| _AssignmentCollection_ <br/> |Optional  <br/> |Microsoft.SharePoint.PowerShell.SPAssignmentCollection  <br/> |Manages objects for the purpose of proper disposal. Use of objects, such as **SPWeb** or **SPSite**, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management. Using the **SPAssignment** object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory. When **SPWeb**, **SPSite**, or **SPSiteAdministration** objects are used, the objects are automatically disposed of if an assignment collection or the **Global** parameter is not used.  <br/> > [!NOTE]> When the **Global** parameter is used, all objects are contained in the global store. If objects are not immediately used, or disposed of by using the **Stop-SPAssignment** command, an out-of-memory scenario can occur.           |
| _Confirm_ <br/> |Optional  <br/> |System.Management.Automation.SwitchParameter  <br/> |Prompts you for confirmation before executing the command. For more information, type the following command: **get-help about_commonparameters** <br/> |
| _SearchApplication_ <br/> |Optional  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchServiceApplicationPipeBind  <br/> |Specifies the search service application that contains the search topology.  <br/> |
| _WhatIf_ <br/> |Optional  <br/> |System.Management.Automation.SwitchParameter  <br/> |Displays a message that describes the effect of the command instead of executing the command. For more information, type the following command: **get-help about_commonparameters** <br/> |
   
## AutoGenParams

|**Parameter**|**Required**|**Type**|**Description**|
|:-----|:-----|:-----|:-----|
|**SearchServiceInstance** <br/> |Required  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchServiceInstancePipeBind  <br/> ||
|**SearchTopology** <br/> |Required  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchTopologyPipeBind  <br/> ||
|**AssignmentCollection** <br/> |Optional  <br/> |Microsoft.SharePoint.PowerShell.SPAssignmentCollection  <br/> ||
|**Confirm** <br/> |Optional  <br/> |System.Management.Automation.SwitchParameter  <br/> ||
|**SearchApplication** <br/> |Optional  <br/> |Microsoft.Office.Server.Search.Cmdlet.SearchServiceApplicationPipeBind  <br/> ||
|**WhatIf** <br/> |Optional  <br/> |System.Management.Automation.SwitchParameter  <br/> ||
   
