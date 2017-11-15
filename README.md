# ShareBook

1.获取书籍借阅列表  http://localhost:8000/bookItem/books   POST方法  参数有str，可以模糊查询书籍名称，作者，上传书籍者姓名；tag，书籍标签；pageSize页码尺寸；pageNo页码

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
