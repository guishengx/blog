title: fruitday应用分析
date: 2015-04-07 13:26:09
tags:
---
#一，启动
##(1)
POST http://wapi.fruitday.com/appApi

request:

```
open_user_id	2264049460
service		appuser.oAuthSignin
sign			bfb22cd7f1192c641c64bb1a008f7627
timestamp		1426577585
```

response:

```
{
    	"connect_id": "37471901bb57ca32f50eb8ad7ff43219"
}
```
##(2)	/appMarketing/get_base_url
GET /appMarketing/get_base_url HTTP/1.1

request:

```
Host	wapi.fruitday.com
Accept-Encoding	gzip, deflate
Accept	*/*
Accept-Language	zh-Hans;q=1
Connection	keep-alive
User-Agent	Fruitday/2015012102 (iPhone; iOS 7.1.2; Scale/2.00)
```
response:

```
{
    	"base_url": "http:\/\/wapi.fruitday.com"
}
```

##(3) 获取主页显示内容
GET	/appMarketing/banner_V150/106092/appStore/i1.5.1

```
response:
    {
    	"rotation": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-06\/1425621486_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733",
    		"type": "2",
    		"target_id": "3680",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-12\/1426150964_pic.jpg",
    		"price": "0",
    		"title": "\u5168\u4ed3",
    		"type": "2",
    		"target_id": "3607",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-09\/1425893225_pic.jpg",
    		"price": "0",
    		"title": "APP\u4e0a\u6d77",
    		"type": "6",
    		"target_id": "1111",
    		"description": "",
    		"page_url": "http:\/\/active.fruitday.com\/sale\/Strawberry_app\/index.html?"
    	}],
    	"banner": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-15\/1423965364_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3694",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-15\/1423965405_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3693",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-03\/1425355423_pic.jpg",
    		"price": "0",
    		"title": "\u5168\u4ed3",
    		"type": "2",
    		"target_id": "2428",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-09\/1425887654_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3664",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-01-20\/1421734304_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733\u6210\u90fd",
    		"type": "2",
    		"target_id": "3524",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-10\/1425957641_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "6",
    		"target_id": "1111",
    		"description": "",
    		"page_url": "http:\/\/active.fruitday.com\/sale\/disney_app\/index.html?"
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-03\/1425357322_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733",
    		"type": "2",
    		"target_id": "2360",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-02\/1425302434_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733\u6210\u90fd",
    		"type": "2",
    		"target_id": "3554",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-03\/1425351613_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u5317\u4eac\u676d\u5dde\u6210\u90fd",
    		"type": "2",
    		"target_id": "3526",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-02\/1425283780_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3265",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-28\/1425115146_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3819",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-02\/1422881678_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733\u6210\u90fd",
    		"type": "2",
    		"target_id": "2321",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-05\/1425563918_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "2",
    		"target_id": "3631",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-28\/1425116577_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u6210\u90fd",
    		"type": "2",
    		"target_id": "3622",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-01-28\/1422444889_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u5317\u4eac\u6df1\u5733",
    		"type": "2",
    		"target_id": "1389",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-01-26\/1422255579_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde\u5317\u4eac\u6df1\u5733",
    		"type": "2",
    		"target_id": "1404",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-26\/1424948573_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u5317\u4eac\u676d\u5dde",
    		"type": "2",
    		"target_id": "3817",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-12\/1426151496_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u5317\u4eac\u676d\u5dde\u6df1\u5733",
    		"type": "2",
    		"target_id": "3872",
    		"description": "",
    		"page_url": ""
    	}],
    	"top_banner": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-16\/1426507066_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77\u676d\u5dde",
    		"type": "6",
    		"target_id": "1111",
    		"description": "",
    		"page_url": "http:\/\/active.fruitday.com\/sale\/kiwi_app\/kiwiindex.html?"
    	}],
    	"mobile_product_list": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-02-17\/1424158993_pic.jpg",
    		"price": "0",
    		"title": "\u624b\u673a\u4e13\u4eab",
    		"type": "2",
    		"target_id": "3838",
    		"description": "",
    		"page_url": ""
    	}],
    	"qiangxian_product_list": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2014-09-05\/1409886640_pic.jpg",
    		"price": "0",
    		"title": "\u62a2\u9c9c\u5566\uff01",
    		"type": "7",
    		"target_id": "121",
    		"description": "",
    		"page_url": ""
    	}],
    	"mix_banner": [{
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-10\/1425954678_pic.jpg",
    		"price": "0",
    		"title": "\u5168\u573a\u6ee1\u8d60",
    		"type": "1",
    		"target_id": "141",
    		"description": "",
    		"page_url": ""
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-02\/1425293254_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "6",
    		"target_id": "1111",
    		"description": "",
    		"page_url": "http:\/\/active.fruitday.com\/sale\/xinren_app\/index.html?"
    	}, {
    		"photo": "http:\/\/cdn.fruitday.com\/images\/2015-03-16\/1426483205_pic.jpg",
    		"price": "0",
    		"title": "\u4e0a\u6d77",
    		"type": "7",
    		"target_id": "121",
    		"description": "",
    		"page_url": ""
    	}]
    }
```

##(4) 获取区域列表

GET http://wapi.fruitday.com/appRegion/getRegionSiteList

response:

```
    [{
    	"region_id": 106092,
    	"region_name": "\u4e0a\u6d77"
    }, {
    	"region_id": 145855,
    	"region_name": "\u4e0a\u6d77\u90ca\u533a"
    }, {
    	"region_id": 1,
    	"region_name": "\u6c5f\u82cf",
    	"son_region": [{
    		"region_id": 14270,
    		"region_name": "\u5e38\u5dde"
    	}, {
    		"region_id": 31710,
    		"region_name": "\u6dee\u5b89"
    	}, {
    		"region_id": 28260,
    		"region_name": "\u8fde\u4e91\u6e2f"
    	}, {
    		"region_id": 2,
    		"region_name": "\u5357\u4eac"
    	}, {
    		"region_id": 23730,
    		"region_name": "\u5357\u901a"
    	}, {
    		"region_id": 17771,
    		"region_name": "\u82cf\u5dde"
    	}, {
    		"region_id": 42749,
    		"region_name": "\u6cf0\u5dde"
    	}, {
    		"region_id": 4536,
    		"region_name": "\u65e0\u9521"
    	}, {
    		"region_id": 46290,
    		"region_name": "\u5bbf\u8fc1"
    	}, {
    		"region_id": 9135,
    		"region_name": "\u5f90\u5dde"
    	}, {
    		"region_id": 49184,
    		"region_name": "\u76d0\u57ce"
    	}, {
    		"region_id": 36177,
    		"region_name": "\u626c\u5dde"
    	}, {
    		"region_id": 39980,
    		"region_name": "\u9547\u6c5f"
    	}]
    }, {
    	"region_id": 54351,
    	"region_name": "\u6d59\u6c5f",
    	"son_region": [{
    		"region_id": 54352,
    		"region_name": "\u676d\u5dde"
    	}, {
    		"region_id": 78239,
    		"region_name": "\u6e56\u5dde"
    	}, {
    		"region_id": 74881,
    		"region_name": "\u5609\u5174"
    	}, {
    		"region_id": 84713,
    		"region_name": "\u91d1\u534e"
    	}, {
    		"region_id": 101443,
    		"region_name": "\u4e3d\u6c34"
    	}, {
    		"region_id": 61841,
    		"region_name": "\u5b81\u6ce2"
    	}, {
    		"region_id": 90123,
    		"region_name": "\u8862\u5dde"
    	}, {
    		"region_id": 81106,
    		"region_name": "\u7ecd\u5174"
    	}, {
    		"region_id": 96033,
    		"region_name": "\u53f0\u5dde"
    	}, {
    		"region_id": 68453,
    		"region_name": "\u6e29\u5dde"
    	}, {
    		"region_id": 93628,
    		"region_name": "\u821f\u5c71"
    	}]
    }, {
    	"region_id": 106340,
    	"region_name": "\u5b89\u5fbd",
    	"son_region": [{
    		"region_id": 116543,
    		"region_name": "\u5b89\u5e86"
    	}, {
    		"region_id": 110702,
    		"region_name": "\u868c\u57e0"
    	}, {
    		"region_id": 140334,
    		"region_name": "\u4eb3\u5dde"
    	}, {
    		"region_id": 142739,
    		"region_name": "\u6c60\u5dde"
    	}, {
    		"region_id": 122473,
    		"region_name": "\u6ec1\u5dde"
    	}, {
    		"region_id": 126555,
    		"region_name": "\u961c\u9633"
    	}, {
    		"region_id": 106341,
    		"region_name": "\u5408\u80a5"
    	}, {
    		"region_id": 114716,
    		"region_name": "\u6dee\u5317"
    	}, {
    		"region_id": 112546,
    		"region_name": "\u6dee\u5357"
    	}, {
    		"region_id": 120049,
    		"region_name": "\u9ec4\u5c71"
    	}, {
    		"region_id": 136386,
    		"region_name": "\u516d\u5b89"
    	}, {
    		"region_id": 113743,
    		"region_name": "\u9a6c\u978d\u5c71"
    	}, {
    		"region_id": 115943,
    		"region_name": "\u94dc\u9675"
    	}, {
    		"region_id": 109303,
    		"region_name": "\u829c\u6e56"
    	}, {
    		"region_id": 130770,
    		"region_name": "\u5bbf\u5dde"
    	}, {
    		"region_id": 144431,
    		"region_name": "\u5ba3\u57ce"
    	}]
    }, {
    	"region_id": 143949,
    	"region_name": "\u5317\u4eac"
    }, {
    	"region_id": 144005,
    	"region_name": "\u5929\u6d25"
    }, {
    	"region_id": 143983,
    	"region_name": "\u6cb3\u5317",
    	"son_region": [{
    		"region_id": 143984,
    		"region_name": "\u77f3\u5bb6\u5e84"
    	}, {
    		"region_id": 144032,
    		"region_name": "\u5eca\u574a"
    	}, {
    		"region_id": 144033,
    		"region_name": "\u627f\u5fb7"
    	}, {
    		"region_id": 144034,
    		"region_name": "\u5510\u5c71"
    	}, {
    		"region_id": 144660,
    		"region_name": "\u4fdd\u5b9a"
    	}, {
    		"region_id": 144668,
    		"region_name": "\u6ca7\u5dde"
    	}, {
    		"region_id": 144677,
    		"region_name": "\u90af\u90f8"
    	}, {
    		"region_id": 144684,
    		"region_name": "\u8861\u6c34"
    	}, {
    		"region_id": 144690,
    		"region_name": "\u79e6\u7687\u5c9b"
    	}, {
    		"region_id": 144694,
    		"region_name": "\u90a2\u53f0"
    	}, {
    		"region_id": 144700,
    		"region_name": "\u5f20\u5bb6\u53e3"
    	}]
    }, {
    	"region_id": 143967,
    	"region_name": "\u6cb3\u5357",
    	"son_region": [{
    		"region_id": 143968,
    		"region_name": "\u90d1\u5dde"
    	}]
    }, {
    	"region_id": 143996,
    	"region_name": "\u5c71\u897f",
    	"son_region": [{
    		"region_id": 143997,
    		"region_name": "\u592a\u539f"
    	}]
    }, {
    	"region_id": 144035,
    	"region_name": "\u5c71\u4e1c",
    	"son_region": [{
    		"region_id": 144036,
    		"region_name": "\u67a3\u5e84"
    	}]
    }, {
    	"region_id": 144039,
    	"region_name": "\u9655\u897f",
    	"son_region": [{
    		"region_id": 144069,
    		"region_name": "\u897f\u5b89"
    	}]
    }, {
    	"region_id": 144252,
    	"region_name": "\u5e7f\u4e1c",
    	"son_region": [{
    		"region_id": 144422,
    		"region_name": "\u6df1\u5733"
    	}, {
    		"region_id": 144261,
    		"region_name": "\u5e7f\u5dde"
    	}, {
    		"region_id": 144274,
    		"region_name": "\u73e0\u6d77"
    	}, {
    		"region_id": 144278,
    		"region_name": "\u6c55\u5934"
    	}, {
    		"region_id": 144285,
    		"region_name": "\u97f6\u5173"
    	}, {
    		"region_id": 144296,
    		"region_name": "\u4f5b\u5c71"
    	}, {
    		"region_id": 144302,
    		"region_name": "\u6c5f\u95e8"
    	}, {
    		"region_id": 144313,
    		"region_name": "\u6e5b\u6c5f"
    	}, {
    		"region_id": 144321,
    		"region_name": "\u8302\u540d"
    	}, {
    		"region_id": 144328,
    		"region_name": "\u8087\u5e86"
    	}, {
    		"region_id": 144334,
    		"region_name": "\u60e0\u5dde"
    	}, {
    		"region_id": 144338,
    		"region_name": "\u6885\u5dde"
    	}, {
    		"region_id": 144341,
    		"region_name": "\u6c55\u5c3e"
    	}, {
    		"region_id": 144345,
    		"region_name": "\u6cb3\u6e90"
    	}, {
    		"region_id": 144347,
    		"region_name": "\u9633\u6c5f"
    	}, {
    		"region_id": 144351,
    		"region_name": "\u6e05\u8fdc"
    	}, {
    		"region_id": 144355,
    		"region_name": "\u4e1c\u839e"
    	}, {
    		"region_id": 144357,
    		"region_name": "\u4e2d\u5c71"
    	}, {
    		"region_id": 144359,
    		"region_name": "\u63ed\u9633"
    	}, {
    		"region_id": 144364,
    		"region_name": "\u4e91\u6d6e"
    	}, {
    		"region_id": 144367,
    		"region_name": "\u6f6e\u5dde"
    	}]
    }, {
    	"region_id": 144387,
    	"region_name": "\u798f\u5efa",
    	"son_region": [{
    		"region_id": 144388,
    		"region_name": "\u798f\u5dde"
    	}, {
    		"region_id": 144396,
    		"region_name": "\u53a6\u95e8"
    	}, {
    		"region_id": 144404,
    		"region_name": "\u6cc9\u5dde"
    	}]
    }, {
    	"region_id": 144412,
    	"region_name": "\u6e56\u5357",
    	"son_region": [{
    		"region_id": 144413,
    		"region_name": "\u957f\u6c99"
    	}]
    }, {
    	"region_id": 144643,
    	"region_name": "\u6e56\u5317",
    	"son_region": [{
    		"region_id": 144644,
    		"region_name": "\u6b66\u6c49"
    	}]
    }]
```

##(5) 



