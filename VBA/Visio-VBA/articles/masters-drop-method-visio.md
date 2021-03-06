---
title: Masters.Drop Method (Visio)
keywords: vis_sdr.chm10816235
f1_keywords:
- vis_sdr.chm10816235
ms.prod: visio
api_name:
- Visio.Masters.Drop
ms.assetid: aff32258-755c-cce3-5f46-e611de6c8f5a
ms.date: 06/08/2017
---


# Masters.Drop Method (Visio)

Creates a new **Master** object by dropping an object onto a receiving object such as a stencil or document, or the **Masters** or **MasterShortcuts** collection.


## Syntax

 _expression_ . **Drop**( **_ObjectToDrop_** , **_xPos_** , **_yPos_** )

 _expression_ A variable that represents a **Masters** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _ObjectToDrop_|Required| **[UNKNOWN]**|The object to drop. While this is typically a Visio object such as a  **Master** , **Shape** , or **Selection** object, it can be any OLE object that provides an **IDataObject** interface.|
| _xPos_|Required| **Integer**|The x-coordinate at which to place the center of the shape's width or PinX.|
| _yPos_|Required| **Integer**|The y-coordinate at which to place the center of the shape's height or PinY.|

### Return Value

Master


## Remarks

Using the  **Drop** method is similar to moving a shape with the mouse. The object dropped ( _ObjectToDrop_) can be a master or a shape on the drawing page.

If  _ObjectToDrop_ is a **Master** , the pin of the master is dropped at the specified coordinates. A master's pin is often, but not necessarily, at its center of rotation.


