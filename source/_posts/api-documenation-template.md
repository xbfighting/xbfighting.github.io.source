---
title: 通用API文档模板
date: 2016-06-18 12:32:02
tags: 
    - API
    - documenation
    - template
---

## API名称

### 1.简要描述

description...

### 2.请求URL

GET https://github.com/login/oauth/authorize

### 3.Request 示例

``` json
{
    "Parameter0": 0,
    "Parameter1": "ONE",
    "Parameter2": [2, 3, 4, 5]
}
```

### 4. Request 参数说明

|   参数  |   格式  |   说明    |   可空    |
| --------   | -----  | ----  |:----:|
| Parameter0   | int32 |      |   N   |
| Parameter1   | string |   |   N   |
| Parameter2   | int32 array |  |   Y   |

### 5. Response 返回示例

``` json
{
    "statu": 1,
    "data": null,
    "message": "SUCCESS"
}
```

### 6. Response 参数说明

|   参数  |   格式  |   说明    |
| --------   | -----  | ----  |
| statu | int32 | description |
| data | object | description |
| message | string | success, error, timeout... |

### 7.备注

---

**[markdown 模板原始文件][1]**


[1]: https://raw.githubusercontent.com/xbfighting/xbfighting.github.io/master/xbfighting.github.io/source/_posts/api-documenation-template.md