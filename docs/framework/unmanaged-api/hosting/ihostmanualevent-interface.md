---
title: IHostManualEvent 接口
ms.date: 03/30/2017
api_name:
- IHostManualEvent
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- IHostManualEvent
helpviewer_keywords:
- IHostManualEvent interface [.NET Framework hosting]
ms.assetid: 300c2661-b7d1-4c39-b080-9ebdef0fd523
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 53aaf4c23861666962e5567a6cf9eb9fffc6292f
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="ihostmanualevent-interface"></a>IHostManualEvent 接口
提供的表示形式的手动重置事件主机的实现。  
  
## <a name="methods"></a>方法  
  
|方法|描述|  
|------------|-----------------|  
|[Reset 方法](../../../../docs/framework/unmanaged-api/hosting/ihostmanualevent-reset-method.md)|重置当前`IHostManualEvent`为非终止状态的实例。|  
|[Set 方法](../../../../docs/framework/unmanaged-api/hosting/ihostmanualevent-set-method.md)|设置当前`IHostManualEvent`发送信号状态的实例。|  
|[Wait 方法](../../../../docs/framework/unmanaged-api/hosting/ihostmanualevent-wait-method.md)|导致当前`IHostManualEvent`等待，直到其拥有的实例或指定的经历的时间量。|  
  
## <a name="requirements"></a>要求  
 **平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** MSCorEE.h  
  
 **库：**作为 MSCorEE.dll 中的资源  
  
 **.NET framework 版本：** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [ICLRSyncManager 接口](../../../../docs/framework/unmanaged-api/hosting/iclrsyncmanager-interface.md)  
 [IHostAutoEvent 接口](../../../../docs/framework/unmanaged-api/hosting/ihostautoevent-interface.md)  
 [IHostSemaphore 接口](../../../../docs/framework/unmanaged-api/hosting/ihostsemaphore-interface.md)  
 [IHostSyncManager 接口](../../../../docs/framework/unmanaged-api/hosting/ihostsyncmanager-interface.md)  
 [承载接口](../../../../docs/framework/unmanaged-api/hosting/hosting-interfaces.md)
