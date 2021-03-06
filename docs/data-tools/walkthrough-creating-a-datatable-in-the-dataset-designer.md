---
title: "Walkthrough: Creating a DataTable in the Dataset Designer | Microsoft Docs"
ms.custom: ""
ms.date: "10/19/2016"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "VB"
  - "CSharp"
  - "C++"
  - "aspx"
helpviewer_keywords: 
  - "DataTable objects, creating"
  - "Dataset Designer, creating data tables"
  - "tables [Visual Studio], creating"
  - "data [Visual Studio], Dataset Designer"
ms.assetid: abf0a2b5-e4e5-422e-97ef-55a0e35a82df
caps.latest.revision: 10
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
robots: noindex,nofollow
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# Walkthrough: Creating a DataTable in the Dataset Designer
This walkthrough explains how to create a <xref:System.Data.DataTable> (without a TableAdapter) using the **Dataset Designer**. For information on creating data tables that include TableAdapters, see [Create and configure TableAdapters](../data-tools/create-and-configure-tableadapters.md).  
  
 Tasks illustrated in this walkthrough include:  
  
-   Creating a new Windows Application project  
  
-   Adding a new dataset to the application  
  
-   Adding a new data table to the dataset  
  
-   Adding columns to the data table  
  
-   Setting the primary key for the table  
  
## Creating a New Windows Application  
  
#### To create a new Windows Application project  
  
1.  From the **File** menu, create a new project.  
  
2.  Choose a programming language in the **Project Types** pane.  
  
3.  Click **Windows Application** in the **Templates** pane.  
  
4.  Name the project `DataTableWalkthrough`, and then click **OK**.  
  
     Visual Studio adds the project to **Solution Explorer** and displays **Form1** in the designer.  
  
## Adding a New Dataset to the Application  
  
#### To add a new dataset item to the project  
  
1.  On the **Project** menu, click **Add New Item**.  
  
     The Add New Item Dialog Box appears.  
  
2.  In the **Templates** box, select **DataSet**.  
  
3.  Click **Add**.  
  
     Visual Studio will add a file called **DataSet1.xsd** to the project and open it in the **Dataset Designer**.  
  
## Adding a New DataTable to the Dataset  
  
#### To add a new data table to the dataset  
  
1.  Drag a **DataTable** from the **DataSet** tab of the **Toolbox** onto the **Dataset Designer**.  
  
     A table named **DataTable1** is added to the dataset.  
  
   
2.  Click the title bar of **DataTable1** and rename it `Music`.  
  
## Adding Columns to the Data Table  
  
#### To add columns to the data table  
  
1.  Right-click the **Music** table. Point to **Add**, and then click **Column**.  
  
2.  Name the column `SongID`.  
  
3.  In the **Properties** window, set the <xref:System.Data.DataColumn.DataType%2A> property to <xref:System.Int16?displayProperty=fullName>.  
  
4.  Repeat this process and add the following columns:  
  
     `SongTitle`: <xref:System.String?displayProperty=fullName>  
  
     `Artist`: <xref:System.String?displayProperty=fullName>  
  
     `Genre`: <xref:System.String?displayProperty=fullName>  
  
## Setting the Primary Key for the Table  
 All data tables should have a primary key. A primary key uniquely identifies a specific record in a data table.  
  
#### To set the primary key of the data table  
  
-   Right-click the **SongID** column, and then click **Set Primary Key**.  
  
     A key icon appears next to the **SongID** column.  
  
## Saving Your Project  
  
#### To save the DataTableWalkthrough project  
  
-   On the **File** menu, click **Save All**.  
  
## See Also  
    
 [Bind controls to data in Visual Studio](../data-tools/bind-controls-to-data-in-visual-studio.md)   
 [Validating Data](validate-data-in-datasets.md)   
 [Saving Data](../data-tools/saving-data.md)   
