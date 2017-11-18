# ShareBook


1.前端页面首先获取js签名信息 
http://localhost:8000/auth/configValue  GET方法

返回结果:
{
    "msg": null,
    "success": true,
    "content": {
        "jsTicket": "xSL77YK3VIDxHzpG2m9bKdV91lIWIa44yNqDOykCny8IIdmtLny0Qt2y20rzrQsZfNvPhpGQzImSwMZpFO5eiZ",
        "signature": "b8d5fa681ab213c204026378e9ad15a1655eef0d",
        "nonceStr": "K12ShareBook",
        "timeStamp": "1510990805",
        "corpId": "dinge5991d3dd910986a",
        "agentId": "135308443"
    }
}

2.根据临时授权码获取用户信息
http://localhost:8000/user/code/{code}   GET方法   {code}为前台获取的临时授权码

返回结果：
{
    "msg": null,
    "success": true,
    "content": {
        "id": 2,
        "userName": "周敏文",
        "password": null,
        "userId": null,
        "corpId": "dinge5991d3dd910986a",
        "department": "[52812301,1,52812299]",
        "createTime": 1510985937413,
        "score": 1,
        "gmtMotifiedTime": null,
        "jobNumber": null,
        "dingId": "$:LWCP_v1:$R2RBA92Bbp74IE4La6nziA==",
        "lastLoginTime": 1510985937843,
        "phone": "13336093345",
        "tempUid": "285ecd5e-3a25-4163-a34f-d5ded4bc06c8",
        "firstLogin": true
    }
}


2.获取书籍首页列表  http://localhost:8000/bookItem/books   POST方法  参数有str，可以模糊查询书籍名称，作者，上传书籍者姓名；tag，书籍标签；pageSize页码尺寸；pageNo页码

返回结果：
{
    "msg": null,
    "success": true,
    "content": {
        "list": [
            {
                "id": 2,
                "name": "书籍名称",
                "description": "书籍描述",
                "publisher": "出版社",
                "doubanUrl": "豆瓣地址",
                "imageUrl": "书籍图片豆瓣地址",
                "bookUploadType": 2,（书籍上传类型，1为扫码上传，2为图片上传）
                "uploadDate": 1510583321000,
                "author": "作者",
                "bookPic": null,
                "status": "1",
                "statusDesc": "可借阅",
                "itemList": null
            },
            {...}
        ],
        "pageSize": 10,
        "pageNo": 1,
        "count": 2
    }
}
