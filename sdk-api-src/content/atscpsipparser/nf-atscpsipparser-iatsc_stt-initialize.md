---
UID: NF:atscpsipparser.IATSC_STT.Initialize
title: IATSC_STT::Initialize (atscpsipparser.h)
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
helpviewer_keywords: ["IATSC_STT interface [Microsoft TV Technologies]","Initialize method","IATSC_STT.Initialize","IATSC_STT::Initialize","IATSC_STTInitialize","Initialize","Initialize method [Microsoft TV Technologies]","Initialize method [Microsoft TV Technologies]","IATSC_STT interface","atscpsipparser/IATSC_STT::Initialize","mstv.iatsc_stt_initialize"]
old-location: mstv\iatsc_stt_initialize.htm
tech.root: mstv
ms.assetid: 8a887c78-a1ea-4b81-b933-f95bd33f13c5
ms.date: 12/05/2018
ms.keywords: IATSC_STT interface [Microsoft TV Technologies],Initialize method, IATSC_STT.Initialize, IATSC_STT::Initialize, IATSC_STTInitialize, Initialize, Initialize method [Microsoft TV Technologies], Initialize method [Microsoft TV Technologies],IATSC_STT interface, atscpsipparser/IATSC_STT::Initialize, mstv.iatsc_stt_initialize
req.header: atscpsipparser.h
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
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IATSC_STT::Initialize
 - atscpsipparser/IATSC_STT::Initialize
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - atscpsipparser.h
api_name:
 - IATSC_STT.Initialize
---

# IATSC_STT::Initialize


## -description

This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>Initialize</b> method initializes the object using captured table section data. This method is called internally by the <a href="/previous-versions/windows/desktop/api/atscpsipparser/nf-atscpsipparser-iatscpsipparser-getstt">IAtscPsipParser::GetSTT</a> method, so applications typically should not call it.

## -parameters

### -param pSectionList [in]

Pointer to the <a href="/previous-versions/windows/desktop/api/mpeg2data/nn-mpeg2data-isectionlist">ISectionList</a> interface of the <b>SectionList</b> object that contains the section data.

### -param pMPEGData [in]

Pointer to the <a href="/previous-versions/windows/desktop/api/mpeg2data/nn-mpeg2data-impeg2data">IMpeg2Data</a> interface of the MPEG-2 Sections and Tables filter.

## -returns

The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_ALREADY_INITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The object is already initialized.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>

## -see-also

<a href="/previous-versions/windows/desktop/api/atscpsipparser/nn-atscpsipparser-iatsc_stt">IATSC_STT Interface</a>