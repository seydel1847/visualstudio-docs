---
title: "IDebugDocumentText2::GetSize | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugDocumentText2::GetSize"
helpviewer_keywords: 
  - "IDebugDocumentText2::GetSize"
ms.assetid: bf515a8f-dcee-4004-8f81-543d547ceaae
caps.latest.revision: 11
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugDocumentText2::GetSize
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugDocumentText2::GetSize](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugdocumenttext2-getsize).  
  
Retrieves the size of the text at this position in the document.  
  
## Syntax  
  
```cpp#  
HRESULT GetSize(   
   ULONG* pcNumLines,  
   ULONG* pcNumChars  
);  
```  
  
```csharp  
int GetSize(   
   ref uint pcNumLines,  
   ref uint pcNumChars  
);  
```  
  
#### Parameters  
 `pcNumLines`  
 [out] Returns the number of lines of text.  
  
 `pcNumChars`  
 [out] Returns the number of characters of text.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 [C++ only] If a particular value is not desired, pass a NULL for the parameter.  
  
 [C# only] Both parameters must be specified.  
  
## See Also  
 [IDebugDocumentText2](../../../extensibility/debugger/reference/idebugdocumenttext2.md)
