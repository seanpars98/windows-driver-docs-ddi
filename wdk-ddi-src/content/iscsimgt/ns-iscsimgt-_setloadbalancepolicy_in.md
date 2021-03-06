---
UID: NS:iscsimgt._SetLoadBalancePolicy_IN
title: _SetLoadBalancePolicy_IN (iscsimgt.h)
description: The SetLoadBalancePolicy_IN structure holds the input data for the SetLoadBalance method.
old-location: storage\setloadbalancepolicy_in.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["SetLoadBalancePolicy_IN structure"]
ms.keywords: "*PSetLoadBalancePolicy_IN, PSetLoadBalancePolicy_IN, PSetLoadBalancePolicy_IN structure pointer [Storage Devices], SetLoadBalancePolicy_IN, SetLoadBalancePolicy_IN structure [Storage Devices], _SetLoadBalancePolicy_IN, iscsimgt/PSetLoadBalancePolicy_IN, iscsimgt/SetLoadBalancePolicy_IN, storage.setloadbalancepolicy_in, structs-iSCSI_d4d805d0-4c3c-4f5e-90ee-9c6bf881dfcf.xml"
req.header: iscsimgt.h
req.include-header: Iscsimgt.h
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
req.typenames: SetLoadBalancePolicy_IN, *PSetLoadBalancePolicy_IN
f1_keywords:
 - _SetLoadBalancePolicy_IN
 - iscsimgt/_SetLoadBalancePolicy_IN
 - PSetLoadBalancePolicy_IN
 - iscsimgt/PSetLoadBalancePolicy_IN
 - SetLoadBalancePolicy_IN
 - iscsimgt/SetLoadBalancePolicy_IN
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - iscsimgt.h
api_name:
 - SetLoadBalancePolicy_IN
---

# _SetLoadBalancePolicy_IN structure


## -description

The SetLoadBalancePolicy_IN structure holds the input data for the SetLoadBalance method.

## -struct-fields

### -field LoadBalancePolicies

A structure that contains the information that is required for setting the load balance policy.

## -remarks

You must implement this class.

## -see-also

<a href="/windows-hardware/drivers/storage/msiscsi-lb-operations-wmi-class">MSiSCSI_LB_Operations WMI Class</a>
