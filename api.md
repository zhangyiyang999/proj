# 校区管理
## 公寓管理
### 添加公寓
#### 请求地址
    /api/partment/add
#### 请求方式
    POST
#### 请求参数
    {
      "branch": "北科", // 所属校区：[字符串：必填]
      "name": "21公寓", // 公寓名称：[字符串：必填]
      "type": "自有", // 公寓类型：[字符串：必填] 自有 | 租赁
      "no": "BK-ZL-001" // 公寓编号：[字符串：必填]
      "expire": "2018-03-01~2021-03-01" // 合同期限:[字符串：必填]
      "count": 23 //宿舍数量: [数值: 必填]
    }
#### 返回数据
	{
      "ret": true, // 错误代码：[布尔：必填] true 无错误 false 有错误
      "errmsg": "", // 错误信息：[字符串：默认为空]
      "data": { // 数据内容
        status："ok", // 存取状态：[字符串：必填] "ok" 成功 "fail" 失败
        msg: "数据存取成功" // 附加信息：[字符串：选填]
      }
	}
