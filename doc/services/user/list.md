# 用户列表

### 功能描述

用户列表


### 请求域名:

测试环境：https://api-eas-test.xxx.cn

### 请求URL:

POST:/api/users

### 安全选项：

|  安全项  |  值   |
| :-----  | :---: |
| 登录授权 | N |
| 签名验证 | N |
| XSS 防御 | Y |

### 请求参数:

| 参数名 | 必填？| 类型 | 说明 |
|:----  |:---|:----- |-----   |
|page_size|N|int|每页显示条数|

### Payload 响应参数:

*仅对不易理解的参数名给出解释，其他请参照`响应示例`。*

| 参数名 | 必填？| 类型 | 说明 |
|:----  |:---|:----- |-----   |


### 返回示例:

**正确时返回:**

```json
{
    "payload": {
        "current_page": 1,
        "data": [
            {
                "id": 1,
                "employee_id": 0,
                "workcode": "013224",
                "teaching_center_ids": "1,2,3,4,5",
                "username": "151********",
                "full_name": "owen",
                "en_full_name": "owen",
                "dd_full_name": "bai（owen）",
                "avatar": "x.jpg",
                "created_at": "2017-09-14 14:15:44",
                "updated_at": "2018-01-20 18:00:48",
                "roles": [
                    {
                        "id": 1,
                        "name": "超级管理员",
                        "description": "超级管理员角色",
                        "created_at": "2018-01-22 16:50:20",
                        "updated_at": null,
                        "pivot": {
                            "user_id": 1,
                            "role_id": 1
                        }
                    },
                    {
                        "id": 2,
                        "name": "管理员",
                        "description": "管理员",
                        "created_at": "2018-01-22 16:50:39",
                        "updated_at": null,
                        "pivot": {
                            "user_id": 1,
                            "role_id": 2
                        }
                    }
                ]
            },
            {
                "id": 3,
                "employee_id": 0,
                "workcode": "058704",
                "username": "13633333333",
                "full_name": "0红",
                "en_full_name": "sop",
                "dd_full_name": "sop",
                "avatar": null,
                "created_at": "2017-10-23 11:54:24",
                "updated_at": "2017-10-23 11:54:33",
                "roles": []
            } 
        ],
        "from": 1,
        "last_page": 398,
        "next_page_url": "http://dev.x.com/api/users?page=2",
        "path": "http://dev.x.com/api/users",
        "per_page": 10,
        "prev_page_url": null,
        "to": 10,
        "total": 3974
    },
    "pager": {
        "current": 1,
        "last": 398,
        "size": 10,
        "total": 3974,
        "form_item": 1,
        "to_item": 10
    },
    "err_code": 0
}
```

**错误时返回:**

