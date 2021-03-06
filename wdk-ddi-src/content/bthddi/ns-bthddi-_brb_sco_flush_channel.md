---
UID: NS:bthddi._BRB_SCO_FLUSH_CHANNEL
title: _BRB_SCO_FLUSH_CHANNEL (bthddi.h)
description: The _BRB_SCO_FLUSH_CHANNEL structure describes a flush operation for a SCO channel.
old-location: bltooth\_brb_sco_flush_channel.htm
tech.root: bltooth
ms.date: 04/27/2018
keywords: ["BRB_SCO_FLUSH_CHANNEL structure"]
ms.keywords: "_BRB_SCO_FLUSH_CHANNEL, _BRB_SCO_FLUSH_CHANNEL structure [Bluetooth Devices], bltooth._brb_sco_flush_channel, bth_structs_d2a9941d-7091-402d-87bc-a5da139dfc1f.xml, bthddi/_BRB_SCO_FLUSH_CHANNEL"
req.header: bthddi.h
req.include-header: Bthddi.h
req.target-type: Windows
req.target-min-winverclnt: Versions:\_Supported in Windows Vista, and later.
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
f1_keywords:
 - _BRB_SCO_FLUSH_CHANNEL
 - bthddi/_BRB_SCO_FLUSH_CHANNEL
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - bthddi.h
api_name:
 - _BRB_SCO_FLUSH_CHANNEL
---

# _BRB_SCO_FLUSH_CHANNEL structure

## -description

The _BRB_SCO_FLUSH_CHANNEL structure describes a flush operation for a SCO channel.

## -struct-fields

### -field Hdr

A [BRB_HEADER](ns-bthddi-_brb_header.md) structure that contains information
     about the current BRB.

### -field BtAddress

The Bluetooth address of the remote device.

### -field ChannelHandle

The handle to the SCO channel to flush.

### -field FlushFlags

Valid flags may be combined using a logical OR operation

#### SCO_FLUSH_DIRECTION_OUT

#### SCO_FLUSH_DIRECTION_IN

## -remarks

To flush a SCO channel, profile drivers should [build and send](/previous-versions/ff536657(v=vs.85)) a [BRB_SCO_FLUSH_CHANNEL](/previous-versions/ff536623(v=vs.85)) request.

All pending data transfer IRPs will be completed with STATUS_REQUEST_ABORTED. In-progress IRPs will be completed normally, with success or failure,depending on whether the Bluetooth driver stack was able to transfer data to or from the remote device.

## -see-also

[BRB_HEADER](ns-bthddi-_brb_header.md)

[BRB_SCO_FLUSH_CHANNEL](/previous-versions/ff536623(v=vs.85))
