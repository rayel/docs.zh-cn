---
title: IXCLRDataProcess::StartEnumModules 方法
ms.date: 01/16/2019
api.name:
- IXCLRDataProcess::StartEnumModules Method
api.location:
- mscordacwks.dll
api.type:
- COM
f1.keywords:
- IXCLRDataProcess::StartEnumModules Method
helpviewer.keywords:
- IXCLRDataProcess::StartEnumModules Method [.NET Framework debugging]
topic_type:
- apiref
author: cshung
ms.author: andrewau
ms.openlocfilehash: a81da147c1483e7649612050f4aba29a2cc63b49
ms.sourcegitcommit: b56d59ad42140d277f2acbd003b74d655fdbc9f1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2019
ms.locfileid: "54416372"
---
# <a name="ixclrdataprocessstartenummodules-method"></a>IXCLRDataProcess::StartEnumModules 方法

提供要枚举的进程的模块的句柄。

[!INCLUDE[debugging-api-recommended-note](../../../../includes/debugging-api-recommended-note.md)]

## <a name="syntax"></a>语法

```
HRESULT StartEnumModules(
    [out] CLRDATA_ENUM *handle
);
```

### <a name="parameters"></a>参数

`handle` [out]枚举模块句柄。

## <a name="remarks"></a>备注

提供的方法属于`IXCLRDataProcess`接口，并对应于虚拟方法表 24 槽。

## <a name="requirements"></a>要求

**平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
**标头：** 无  
**库：** 无  
**.NET Framework 版本：**[!INCLUDE[net_current_v47plus](../../../../includes/net-current-v47plus.md)]  

## <a name="see-also"></a>请参阅

- [CLRDataSourceType 枚举](../../../../docs/framework/unmanaged-api/debugging/clrdatasourcetype-enumeration.md)
- [调试](../../../../docs/framework/unmanaged-api/debugging/index.md)
- [IXCLRDataProcess 接口](../../../../docs/framework/unmanaged-api/debugging/ixclrdataprocess-interface.md)
