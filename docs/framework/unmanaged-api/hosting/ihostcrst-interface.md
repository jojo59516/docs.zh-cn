---
title: IHostCrst 接口
ms.date: 03/30/2017
api_name:
- IHostCrst
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- IHostCrst
helpviewer_keywords:
- IHostCrst interface [.NET Framework hosting]
ms.assetid: ac298ebd-0815-47e4-a823-30b31baab903
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 88f2ef8299911905d651ad5c3076dc9c74f397f8
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="ihostcrst-interface"></a>IHostCrst 接口
用作主机的表示形式的线程处理关键部分。  
  
## <a name="methods"></a>方法  
  
|方法|描述|  
|------------|-----------------|  
|[Enter 方法](../../../../docs/framework/unmanaged-api/hosting/ihostcrst-enter-method.md)|进入临界区。|  
|[Leave 方法](../../../../docs/framework/unmanaged-api/hosting/ihostcrst-leave-method.md)|离开临界区。|  
|[SetSpinCount 方法](../../../../docs/framework/unmanaged-api/hosting/ihostcrst-setspincount-method.md)|设置临界区的重试次数。|  
|[TryEnter 方法](../../../../docs/framework/unmanaged-api/hosting/ihostcrst-tryenter-method.md)|若要立即输入关键部分中，以及报告是成功还是失败的尝试。|  
  
## <a name="remarks"></a>备注  
 `IHostCrst` 允许公共语言运行时 (CLR) 与主机的表示形式关键部分，直接进行通信，而不是如使用 Win32 函数`EnterCriticalSection`或`LeaveCriticalSection`。  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** MSCorEE.h  
  
 **库：**作为 MSCorEE.dll 中的资源  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [ICLRSyncManager 接口](../../../../docs/framework/unmanaged-api/hosting/iclrsyncmanager-interface.md)  
 [IHostSyncManager 接口](../../../../docs/framework/unmanaged-api/hosting/ihostsyncmanager-interface.md)  
 [承载接口](../../../../docs/framework/unmanaged-api/hosting/hosting-interfaces.md)
