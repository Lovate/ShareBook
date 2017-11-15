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
                "name": "ナミヤ雑貨店の奇蹟",
                "description": "现代人内心流失的东西，这家杂货店能帮你找回——\n僻静的街道旁有一家杂货店，只要写下烦恼投进卷帘门的投信口，第二天就会在店后的牛奶箱里得到回答。\n因男友身患绝症，年轻女孩静子在爱情与梦想间徘徊；克郎为了音乐梦想离家漂泊，却在现实中寸步难行；少年浩介面临家庭巨变，挣扎在亲情与未来的迷茫中……\n他们将困惑写成信投进杂货店，随即奇妙的事情竟不断发生。\n生命中的一次偶然交会，将如何演绎出截然不同的人生？\n如今回顾写作过程，我发现自己始终在思考一个问题：站在人生的岔路口，人究竟应该怎么做？我希望读者能在掩卷时喃喃自语：我从未读过这样的小说。——东野圭吾",
                "publisher": "南海出版公司",
                "doubanUrl": "https://book.douban.com/subject/25862578/",
                "imageUrl": "https://img3.doubanio.com/mpic/s27264181.jpg",
                "bookUploadType": 2,
                "uploadDate": 1510583321000,
                "author": "[日] 东野圭吾,",
                "bookPic": null,
                "status": "1",
                "statusDesc": "可借阅",
                "itemList": null
            },
            {
                "id": 5,
                "name": "爱在西元前",
                "description": "没有人会在束缚状态下还能在汉谟拉比法典中寻找自由主义。如果不小心落进爱情陷阱可能会遇到麻烦，这话法典上没有刻写。很抱歉虽然没刻写而我还是这么做了――因为我是一个老实的人。好玩吧，真好玩，爱情成为一场智力角逐，床第之欢就成了多余的累赘。在遥远的北方桤树林里，湖水这面镜子，仍能看见你在苏美尔两河流域天天用楔形文字书写着巴比伦的伟大。作为女神伊什塔尔的化身，你这个女祭司知识渊博，让我这个野蛮人佩服得五体投地。于是我带足剑齿虎肉做的干粮，不远万里的来到你的国家打算把你抢回去。开心吧，一切如你所愿，但你千算万算却没算到一个招风耳歌手用一首流行歌曲提前点破了所有宿命，于是……",
                "publisher": "二十一世纪出版社",
                "doubanUrl": "https://book.douban.com/subject/1002323/",
                "imageUrl": "https://img3.doubanio.com/mpic/s1158775.jpg",
                "bookUploadType": 1,
                "uploadDate": 1510655939000,
                "author": "周杰",
                "bookPic": null,
                "status": "1",
                "statusDesc": "可借阅",
                "itemList": null
            }
        ],
        "pageSize": 10,
        "pageNo": 1,
        "count": 2
    }
}
