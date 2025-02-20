---
UID: NF:strmif.IIPDVDec.put_IPDisplay
title: IIPDVDec::put_IPDisplay (strmif.h)
description: The put_IPDisplay method sets the decoding resolution.
helpviewer_keywords: ["IIPDVDec interface [DirectShow]","put_IPDisplay method","IIPDVDec.put_IPDisplay","IIPDVDec::put_IPDisplay","IIPDVDecput_IPDisplay","dshow.iipdvdec_put_ipdisplay","put_IPDisplay","put_IPDisplay method [DirectShow]","put_IPDisplay method [DirectShow]","IIPDVDec interface","strmif/IIPDVDec::put_IPDisplay"]
old-location: dshow\iipdvdec_put_ipdisplay.htm
tech.root: dshow
ms.assetid: c89970f8-b515-409b-af75-b1af65a8f94e
ms.date: 4/26/2023
ms.keywords: IIPDVDec interface [DirectShow],put_IPDisplay method, IIPDVDec.put_IPDisplay, IIPDVDec::put_IPDisplay, IIPDVDecput_IPDisplay, dshow.iipdvdec_put_ipdisplay, put_IPDisplay, put_IPDisplay method [DirectShow], put_IPDisplay method [DirectShow],IIPDVDec interface, strmif/IIPDVDec::put_IPDisplay
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IIPDVDec::put_IPDisplay
 - strmif/IIPDVDec::put_IPDisplay
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IIPDVDec.put_IPDisplay
---

# IIPDVDec::put_IPDisplay


## -description

\[The feature associated with this page, [DirectShow](/windows/win32/directshow/directshow), is a legacy feature. It has been superseded by [MediaPlayer](/uwp/api/Windows.Media.Playback.MediaPlayer) and [IMFMediaEngine](/windows/win32/api/mfmediaengine/nn-mfmediaengine-imfmediaengine). **MediaPlayer** and **IMFMediaEngine** have been optimized for Windows 10 and Windows 11. Microsoft strongly recommends that new code use **MediaPlayer** and **IMFMediaEngine** instead of **DirectShow**, when possible. Microsoft suggests that existing code that uses the legacy APIs be rewritten to use the new APIs if possible.\]

The <code>put_IPDisplay</code> method sets the decoding resolution.

## -parameters

### -param displayPix [in]

Member of the <a href="/windows/desktop/api/strmif/ne-strmif-_dvresolution">DVDECODERRESOLUTION</a> enumerated type, specifying the decoding resolution. The meaning of this value depends on whether the current format is NTSC or PAL. The filter determines at run time which format applies, based on the media type.

## -returns

Returns S_OK if successful; otherwise, returns E_FAIL or another error code.

## -remarks

This method will fail if the filter is already streaming media data.

## -see-also

<a href="/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="/windows/desktop/api/strmif/nn-strmif-iipdvdec">IIPDVDec Interface</a>