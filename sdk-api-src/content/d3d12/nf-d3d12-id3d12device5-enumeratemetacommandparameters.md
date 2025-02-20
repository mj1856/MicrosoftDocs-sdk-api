---
UID: NF:d3d12.ID3D12Device5.EnumerateMetaCommandParameters
title: ID3D12Device5::EnumerateMetaCommandParameters (d3d12.h)
description: Queries reflection metadata about the parameters of the specified meta command.
helpviewer_keywords: ["EnumerateMetaCommandParameters","EnumerateMetaCommandParameters method","EnumerateMetaCommandParameters method","ID3D12Device5 interface","ID3D12Device5 interface","EnumerateMetaCommandParameters method","ID3D12Device5.EnumerateMetaCommandParameters","ID3D12Device5::EnumerateMetaCommandParameters","d3d12/ID3D12Device5::EnumerateMetaCommandParameters","direct3d12.id3d12device5_enumeratemetacommandparameters"]
old-location: direct3d12\id3d12device5_enumeratemetacommandparameters.htm
tech.root: direct3d12
ms.assetid: EA4DD3FE-E11A-4F1C-A765-4B1FCA71FB4B
ms.date: 12/05/2018
ms.keywords: EnumerateMetaCommandParameters, EnumerateMetaCommandParameters method, EnumerateMetaCommandParameters method,ID3D12Device5 interface, ID3D12Device5 interface,EnumerateMetaCommandParameters method, ID3D12Device5.EnumerateMetaCommandParameters, ID3D12Device5::EnumerateMetaCommandParameters, d3d12/ID3D12Device5::EnumerateMetaCommandParameters, direct3d12.id3d12device5_enumeratemetacommandparameters
f1_keywords:
- d3d12/ID3D12Device5.EnumerateMetaCommandParameters
dev_langs:
- c++
req.header: d3d12.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D12.h
api_name:
- ID3D12Device5.EnumerateMetaCommandParameters
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D12Device5::EnumerateMetaCommandParameters


## -description


Queries reflection metadata about the parameters of the specified meta command.


## -parameters




### -param CommandId [in]

Type: <b>REFIID</b>

A reference to the globally unique identifier (GUID) of the meta command whose parameters you wish to be returned in <i>pParameterDescs</i>.


### -param Stage [in]

Type: <b>D3D12_META_COMMAND_PARAMETER_STAGE</b>

A <a href="https://msdn.microsoft.com/1A3278EE-5D46-4E18-9F10-47001506C3DC">D3D12_META_COMMAND_PARAMETER_STAGE</a> specifying the stage of the parameters that you wish to be included in the query.


### -param pTotalStructureSizeInBytes [out, optional]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">UINT</a>*</b>

An optional pointer to a <a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">UINT</a> containing the size of the structure containing the parameter values, which you pass when creating/initializing/executing the meta command, as appropriate.


### -param pParameterCount [in, out]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">UINT</a>*</b>

A pointer to a <a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">UINT</a> containing the number of parameters to query for. This field determines the size of the <i>pParameterDescs</i> array, unless <i>pParameterDescs</i> is <b>nullptr</b>.


### -param pParameterDescs [out, optional]

Type: <b>D3D12_META_COMMAND_PARAMETER_DESC*</b>

An optional pointer to an array of  <a href="https://msdn.microsoft.com/F4314919-B7E1-4628-867D-462F8F9A48FA">D3D12_META_COMMAND_PARAMETER_DESC</a> containing the descriptions of the parameters. Pass <b>nullptr</b> to have the parameter count returned in <i>pParameterCount</i>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Mt847457(v=VS.85).aspx">ID3D12Device5</a>
 

 

