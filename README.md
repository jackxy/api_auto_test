**小滴课堂接口自动化测试例子-update 2020-07**

**接口域名：https://api.xdclass.net**

<hr>


### 首页模块


#### 分类列表

请求方式：get

路径：/pub/api/v1/web/all_category

请求头：无

请求参数：无

响应协议：

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |

响应例子

```
{
    "code":0,
    "data":[
        {
            "id":1,
            "name":"后端&架构",
            "createTime":"2017-11-12T01:11:11.000+0000",
            "pid":null,
            "del":null,
            "level":null,
            "subCategoryList":[
                {
                    "id":95,
                    "name":"必备基础",
                    "createTime":"2020-06-12T03:33:55.000+0000",
                    "pid":1,
                    "del":null,
                    "level":1,
                    "videoList":null
                }
            ],
            "videoList":[
                {
                    "id":52,
                    "title":"ssm新版SpringBoot2.3/spring5/mybatis3",
                    "summary":"https://file.xdclass.net/video/2020/SSM/xqt-ssm.png",
                    "price":6800,
                    "online":1,
                    "point":9.8,
                    "level":3,
                    "hours":34,
                    "cover_img":"https://file.xdclass.net/video/2020/SSM/zt-ssm.png",
                    "view_num":19145,
                    "buy_num":369,
                    "author_id":1,
                    "create_time":"2020-06-15 10:14:00",
                    "update_time":"2020-06-27 04:29:42",
                    "old_price":19800,
                    "c_id":null,
                    "cp_id":null,
                    "learn_base":"需要有javaweb基础||项目实战需要有HTML+JS基础",
                    "learn_result":"掌握 SpringBoot2.3框架包括接口开发.跨域配置等 和 公司项目开发||Mybaits3框架 增删改查，复杂多表关联查询、多级缓存等||Spring5框架包括自动注入,XML和常用注解，切面编程AOP，CGlib动态代理等||急速掌握 Vue2.6 + VueCli4.3 + CubeUI框架，VSCode编辑器和ES6语法||独立开发综合实战包括前端-后端-部署上线，达到全栈工程师水平||项目性能优化+Jmeter接口压测，QPS1万+",
                    "total_episode":203,
                    "record_state":null,
                    "pre_remark":null,
                    "player_order":"2",
                    "share":0
                }
            ]
        }
    ],
    "msg":null
}
```







<hr>



#### 视频卡片

请求方式：get

路径：/pub/api/v1/web/index_card

请求头：无

请求参数：无

响应协议：

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |

响应例子

```
{
    "code":0,
    "data":[],
    "msg":null
}
```





<hr>

#### 视频详情

请求方式：get

路径：/pub/api/v1/web/video_detail?video_id=53

请求头：无

请求参数

| 参数名 | 解释 |
| ------ | ---- |
| 视频id |      |

响应协议：

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |

响应例子

```
{
    "code":0,
    "data":{
        "chapter_list":[
            {
                "id":1101,
                "videoId":53,
                "title":"小滴课堂新版Javaweb 课程大纲概要",
                "ordered":1,
                "createTime":"2020-06-10T09:12:02.000+0000",
                "episodeList":[
                    {
                        "id":102701,
                        "title":"小滴课堂新版javaweb课程介绍和学后水平",
                        "num":1,
                        "duration":null,
                        "free":0,
                        "coverImg":null,
                        "videoId":53,
                        "summary":null,
                        "createTime":null,
                        "chapterId":1101,
                        "aliyunId":null,
                        "ordered":1,
                        "note":null,
                        "hwyunId":"032857664d902a3ee673b263cac4dc05"
                    }
                ]
            }
        ],
        "author":{
            "head_img":"https://thirdwx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTJoC7iczcqvp78u1f0HrJicdrs5KXX81udJU4339X5Q2YKJwlWJUiavOSex0trNqOy7TduHrXgbCTzMQ/132",
            "profile":"前阿里资深工程师||小滴课堂技术负责人",
            "name":"小D",
            "author_id":1
        },
        "video":{
            "id":53,
            "title":"新版JavaWeb零基础到实战专题课程",
            "summary":"https://file.xdclass.net/video/2020/javaweb/lbt-javaweb.png",
            "price":4900,
            "online":1,
            "point":9.2,
            "level":2,
            "hours":19,
            "cover_img":"https://file.xdclass.net/video/2020/javaweb/zt-javaweb.png",
            "view_num":2879,
            "buy_num":993,
            "author_id":1,
            "create_time":"2020-03-05 10:14:00",
            "update_time":"2020-06-27 08:57:17",
            "old_price":6900,
            "c_id":6,
            "cp_id":1,
            "learn_base":"只需要javase+Mysql ||简单的HTML/JS前端基础||上面的基础不会也没关系,联系客服小姐姐 都有对应教程",
            "learn_result":"掌握Http协议+新版Servlet3.0,和javaweb全部核心知识||掌握JDBC核心技术、ApacheDBUils和数据库连接池,项目包构建管理工具Maven3.X||掌握Maven3.x+Mysql+IDEA+Servlet3.0+Tomcat9开发项目实战",
            "total_episode":96,
            "record_state":1,
            "pre_remark":null,
            "player_order":"2",
            "share":0
        }
    },
    "msg":null
}
```




<hr>





### 用户模块



#### 用户登录

请求方式：post

路径：/pub/api/v1/web/web_login

请求头：

| 请求头       | 解释                              |
| ------------ | --------------------------------- |
| Content-Type | application/x-www-form-urlencoded |

请求参数

| 参数名 | 解释       |
| ------ | ---------- |
| phone  | 注册手机号 |
| pwd    | 响应数据   |

请求例子

```
phone = 13113777555
pwd = 1234567890
```



响应协议

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |



响应例子

```
{
    "code": 0,
    "data": {
    		//用户头像
        "head_img": "https://xd-video-pc-img.oss-cn-beijing.aliyuncs.com/xdclass_pro/default/head_img/21.jpeg",

				//用户名称
				"name": "dasdadasd111",
        
        //登录成功的令牌
        "token": "xdclasseyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ4ZGNsYXNzIiwicm9sZXMiOiIxLDIiLCJpbWciOiJodHRwczovL3hkLXZpZGVvLXBjLWltZy5vc3MtY24tYmVpamluZy5hbGl5dW5jcy5jb20veGRjbGFzc19wcm8vZGVmYXVsdC9oZWFkX2ltZy8yMS5qcGVnIiwiaWQiOjY3NTAyMiwibmFtZSI6ImRhc2RhZGFzZDExMSIsImlhdCI6MTU5MzMxMTM0NCwiZXhwIjoxNTkzOTE2MTQ0fQ.QbeedfEYPE8inm1wY7xoYYbr_z8qEap8EK0NMjk0djU"
    },
    "msg": null
}
```





<hr>



#### 用户个人信息

请求方式：get

路径：/pub/api/v1/web/user_info

请求头：

| 请求头                | 解释 |
| --------------------- | ---- |
| token |登录接口返回token      |

请求参数：无

响应协议

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |



响应例子

```
{
    "code": 0,
    "data": {
        "id": 675022,
        "vipRank": 0,
        "openid": null,
        "unionid": null,
        "name": "dasdadasd111",
        "headImg": "https://xd-video-pc-img.oss-cn-beijing.aliyuncs.com/xdclass_pro/default/head_img/21.jpeg",
        "phone": "13113777555",
        "signType": 1,
        "email": null,
        "sign": "高级码率",
        "sex": 1,
        "city": "中国",
        "createTime": "2020-06-10T12:42:46.000+0000",
        "points": 10,
        "roles": "1",
        "learnTime": 0,
        "userPay": {
            "id": 11895,
            "appid": "wxdn1150civ35jo88e",
            "appsecret": "q3l4fz2hck13lcuooyw06jp2y422t837",
            "openAppid": null,
            "openAppsecret": null,
            "key": "ZV15f61k97KR82920fMHSHF079Z703g8",
            "merchId": "4122175525",
            "userId": 675022,
            "createTime": "2020-06-10 08:42:46",
            "custom": null,
            "domain": "http://api.xdclass.net"
        },
        "nameWithEncode": "dasdadasd111"
    },
    "msg": null
}
```





<hr>

#### 我的订单

请求方式：get

路径：/user/api/v1/order/find_orders

请求头：

| 请求头                | 解释 |
| --------------------- | ---- |
| token |登录接口返回的token值 |

请求参数：无

响应协议

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |



响应例子

```
{
    "code":0,
    "data":{
        "total":4,
        "data":[
            {
                "id":49189,
                "state":0,
                "nickname":"131",
                "price":1980,
                "hours":3,
                "redeemCode":null,
                "out_trade_no":"234bede23dc344fab5b32df067a0bedf",
                "create_time":"2020-06-08T12:21:47.000+0000",
                "head_img":"https://xd-video-pc-img.oss-cn-beijing.aliyuncs.com/xdclass_pro/default/head_img/15.jpeg",
                "video_id":32,
                "video_title":"新版Maven3.5+Nexus私服搭建全套核心技术",
                "video_img":"https://xdvideo-file.oss-cn-shenzhen.aliyuncs.com/video/2020/maven/%E5%AE%98%E7%BD%91%E4%B8%BB%E5%9B%BE-mawen.png",
                "user_id":675022,
                "current_episode":0,
                "view_num":10125,
                "buy_num":88,
                "total_episode":28
            },
            {
                "id":49190,
                "state":0,
                "nickname":"131",
                "price":2980,
                "hours":5,
                "redeemCode":null,
                "out_trade_no":"d681f7bf903642b8adfcf5c607e532d2",
                "create_time":"2020-06-08T12:21:47.000+0000",
                "head_img":"https://xd-video-pc-img.oss-cn-beijing.aliyuncs.com/xdclass_pro/default/head_img/15.jpeg",
                "video_id":1,
                "video_title":"SpringBoot+Websocket打造实时聊天/股票行情系统",
                "video_img":"https://xd-video-pc-img.oss-cn-beijing.aliyuncs.com/xdclass_pro/video/1807/sp_websocket.png",
                "user_id":675022,
                "current_episode":0,
                "view_num":9330,
                "buy_num":372,
                "total_episode":20
            }
        ],
        "total_page":1,
        "current_page":1
    },
    "msg":null
}
```





<hr>

### 收藏模块



#### 新增收藏

请求方式：post

路径：/user/api/v1/favorite/save

请求头：

| 请求头                | 解释 |
| --------------------- | ---- |
| token |   登录接口返回的token值   |

请求参数

| 参数名   | 解释       |
| -------- | ---------- |
| video_id | 收藏的视频id |

响应协议

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |



响应例子

```
{
    "code": 0,
    "data": {
        "id": null,
        "videoId": 50,
        "userId": 675022,
        "createTime": "2020-06-28T03:00:42.778+0000"
    },
    "msg": null
}
```





<hr>

#### 我的收藏

请求方式：get

路径：/user/api/v1/favorite/page

请求头：

| 请求头                | 解释 |
| --------------------- | ---- |
| token |   登录接口返回的token值   |

请求参数：无

响应协议

| 参数名 | 解释              |
| ------ | ----------------- |
| code   | 状态码 0 表示成功 |
| data   | 响应数据          |
| msg    | 描述信息          |



响应例子

```
{
    "code":0,
    "data":{
        "total":1,
        "data":[
            {
                "id":53,
                "title":"新版JavaWeb零基础到实战专题课程",
                "summary":null,
                "price":4900,
                "online":null,
                "point":9.2,
                "level":4,
                "hours":null,
                "cover_img":"https://file.xdclass.net/video/2020/javaweb/zt-javaweb.png",
                "view_num":2917,
                "buy_num":993,
                "author_id":null,
                "create_time":"2020-06-28 11:05:21",
                "update_time":null,
                "old_price":6900,
                "c_id":null,
                "cp_id":null,
                "learn_base":null,
                "learn_result":null,
                "total_episode":null,
                "record_state":null,
                "pre_remark":null,
                "player_order":null,
                "share":null,
                "favorite_id":2381
            }
        ],
        "total_page":1,
        "current_page":1
    },
    "msg":null
}
```

