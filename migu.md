#酷镜接口文档


>此文档为酷镜营养师提供咪咕语音识别、录入、推荐模块的接口调用及返回值等。

### 版本号
* **v1.0.1**

### 文档目录
#### 1. 语音菜谱推荐接口
#### 2. 语音分析菜品接口



###*1、语音菜谱推荐接口*
####功能说明：
语音模块-推荐

根据语音的分析用户记录（推荐），返回的数据根据用户语义解析后推荐一天(一周、一餐)的餐食结果
####接口地址：
* `URL`: /getNutritionByName?value=我本周吃点什么&app_key=APP的key

####请求参数：
```
[{
	"weight": 50.0,
	"sexName": "女",
	"age": 20,
	"height": 165.0
	"id":121
}]
```
####类型
JSON
####请求方式：
POST
####返回值：
```
{
    "data": {
        "2019-07-20": {
            "breakfast": [
                [
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fce3d9057c393773ef.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=eBMKJU5eKiVVMHznkvW%2BhiceS98%3D",
                        "name": "香菇瘦肉粥",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 58.1,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 2.18,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 3.86,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 4.2,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 1.11,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 750.09,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            },
                            {
                                "value": 0.3,
                                "name": "fe",
                                "desc": "铁",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2fe5fce3d9057c393773ef"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5f9e3d9057c393770fa.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=Oid8FdCEd0rqjDkvcV4PGG55%2Fik%3D",
                        "name": "泡菜煎饼",
                        "weight": 150,
                        "ingredients": [
                            {
                                "value": 170.12,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 7.85,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 5.2,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 25.37,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 2.52,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 0.17,
                                "name": "vitaminB1",
                                "desc": "维生素B1",
                                "unit": "毫克"
                            },
                            {
                                "value": 38.31,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2fe5f9e3d9057c393770fa"
                    }
                ]
            ],
            "lunch": [
                [
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73054cae0207708612d1.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=0YECvr9VWgYKo8NOuGd9PNBPRCA%3D",
                        "name": "素卤咸豆花",
                        "weight": 215.55770331898648,
                        "ingredients": [
                            {
                                "value": 198.83,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 14.37,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 8.97,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 19.05,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 3.98,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 432.73,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            },
                            {
                                "value": 15.64,
                                "name": "fe",
                                "desc": "铁",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73054cae0207708612d1"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73974cae02077086288f.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=r%2B7CbLNpNG%2FjZcUjI7sAERdhL9c%3D",
                        "name": "干豆腐炒金针菇",
                        "weight": 49.976883639035066,
                        "ingredients": [
                            {
                                "value": 193.79,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 23.06,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 10.23,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 6.03,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 3.65,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 0.12,
                                "name": "vitaminC",
                                "desc": "维生素C",
                                "unit": "毫克"
                            },
                            {
                                "value": 504.16,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73974cae02077086288f"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73414cae020770861c96.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=tykURvq8dnW5mN6Oj%2Bs1ZA5R2ZI%3D",
                        "name": "枣香杂面发糕",
                        "weight": 150,
                        "ingredients": [
                            {
                                "value": 347.69,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 12.49,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 2.02,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 74.23,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 4.49,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 39.44,
                                "name": "vitaminC",
                                "desc": "维生素C",
                                "unit": "毫克"
                            },
                            {
                                "value": 2.79,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73414cae020770861c96"
                    }
                ]
            ],
            "dinner": [
                [
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73854cae0207708625f0.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=TldXGDW3D9niqxUK%2FkEtUbaYmLs%3D",
                        "name": "鸡爪炖土豆",
                        "weight": 178.60156988879066,
                        "ingredients": [
                            {
                                "value": 251.29,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 12.88,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 12.96,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 22.83,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 3.42,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 35.27,
                                "name": "vitaminC",
                                "desc": "维生素C",
                                "unit": "毫克"
                            },
                            {
                                "value": 3401.89,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73854cae0207708625f0"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d742a4cae020770863f3f.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=CZ4GmlbqeaqJnO7TDGcV34X%2B77I%3D",
                        "name": "白菜炒土豆片",
                        "weight": 418.72299521129094,
                        "ingredients": [
                            {
                                "value": 209.63,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 8.18,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 0.88,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 45.7,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 4.33,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 71.05,
                                "name": "vitaminC",
                                "desc": "维生素C",
                                "unit": "毫克"
                            },
                            {
                                "value": 113.65,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d742a4cae020770863f3f"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73d74cae020770863224.jpg?Expires=1563525258&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=5%2Fx9xAERsYzbT95tvFNBH1Ji0HY%3D",
                        "name": "糯米红枣新吃法",
                        "weight": 150,
                        "ingredients": [
                            {
                                "value": 292.09,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 4.58,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 0.53,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 67.54,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 0.56,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 5.66,
                                "name": "vitaminA",
                                "desc": "维生素A",
                                "unit": "微克"
                            },
                            {
                                "value": 1.69,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73d74cae020770863224"
                    }
                ]
            ]
        },
        .....
    },
    "message": "成功",
    "status": "ok"
}

```

####请求值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|weight|double|体重(必填)|
|sexName|string|性别(必填)|
|age|int|年龄(必填)|
|height|double|身高(必填)|
|id|int|用户ID(必填)|

* 所有可选参数都可以传空值

####返回值说明
#####data

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|time|结构2|一天当中三餐的集合|

#####结构2

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|breakfast|结构3|早餐|
|lunch|结构3|午餐|
|dinner|结构3|晚餐|


#####结构3
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|id|string|菜品id|
|name|string|菜品名称|
|image|string|菜品图片|
|weight|double|菜品重量|
|ingredients|结构5|营养元素集合|


#####结构5
| 字段名称   | 类型 | 说明 ： <mark>以下营养元素都为每100克的</mark> |
| ------- | --- | :---:  |
|value	|double| 元素值|
|name	|string| 元素名称|
|desc|	string|	元素名称(中文)|
|unit|	string|	单位|


###*2、语音分析菜品接口*
####功能说明：
语音模块-记录

根据一段文本文字返回文本中的`食物`与对应`重量`，集合中包含相似的5道菜品，识别概率从高到底。开发者只需要从集合中取出第一个元素作为识别后的菜品即可，其余菜品可以做用户手动选择项，
####接口地址:

* `URL`: /getNutritionByName?value=我今天早上吃了一碗粥中午吃了200克鱼香肉丝和一碗大米饭&app_key=APP的key

####请求参数：
	{
	  "weight": 70.0, 
	  "sexName": "男",
	  "age": 27,
	  "height": 171.0,
	  "id":1
	}
####类型
JSON
####请求方式：
POST
####返回值：
```
{
    "data": {
        "2019-07-19": {
            "breakfast": [
                [
                    {
                        "image": null,
                        "name": "粥",
                        "ingredients": [
                            {
                                "value": 141,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 3.3,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 0.9,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 29.7,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 0.3,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 8.4,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            },
                            {
                                "value": 0.3,
                                "name": "fe",
                                "desc": "铁",
                                "unit": "毫克"
                            }
                        ],
                        "weight": 300,
                        "id": "5b8fbb67f99ffbe3ae5e22fd"
                    }
                ]
            ],
            "lunch": [
                [
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d730e4cae02077086146e.jpg?Expires=1563525497&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=PQu9cATIS994nPcxF1M6u141bE4%3D",
                        "name": "鱼香肉丝",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 549.78,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 16.79,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 45.58,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 18.44,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 0.58,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 0.26,
                                "name": "vitaminB1",
                                "desc": "维生素B1",
                                "unit": "毫克"
                            },
                            {
                                "value": 809.1,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d730e4cae02077086146e"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d736a4cae020770862285.jpg?Expires=1563525497&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=0in2CqflLgq%2FRzyLq0IcBHshlD0%3D",
                        "name": "鱼香肉丝",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 367.57,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 13.39,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 25.55,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 26.61,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 6.38,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 2399.39,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            },
                            {
                                "value": 233.64,
                                "name": "ca",
                                "desc": "钙",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d736a4cae020770862285"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73c44cae020770862fba.jpg?Expires=1563525497&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=I9mgj%2B%2BMlPZpNMYt6sgNomIkBWQ%3D",
                        "name": "鱼香肉丝",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 205.05,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 25.41,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 7.68,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 9.95,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 1.72,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 483.96,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            },
                            {
                                "value": 4.64,
                                "name": "fe",
                                "desc": "铁",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73c44cae020770862fba"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d740c4cae020770863996.jpg?Expires=1563525497&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=ss5lBuJo%2FzM5UYv6183rfZ2df%2Bs%3D",
                        "name": "-->鱼香肉丝烧土豆",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 209.94,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 21.48,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 0.51,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 31.27,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 2.11,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 2.29,
                                "name": "vitaminE",
                                "desc": "维生素E",
                                "unit": "毫克"
                            },
                            {
                                "value": 4018.6,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d740c4cae020770863996"
                    },
                    {
                        "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73084cae020770861346.jpg?Expires=1563525497&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=ncA4RkusS4qAgmonq7db8YsJhnk%3D",
                        "name": "鱼香鸡丝",
                        "weight": 200,
                        "ingredients": [
                            {
                                "value": 167.29,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 18.51,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 3.48,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 17.06,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 1.92,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 320.22,
                                "name": "vitaminA",
                                "desc": "维生素A",
                                "unit": "微克"
                            },
                            {
                                "value": 1040.19,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "id": "5d2d73084cae020770861346"
                    }
                ],
                [
                    {
                        "image": "http://app.oramiro.com:8082/oramirror_cloud/group/114997/1464266101204.jpg",
                        "name": "米饭",
                        "ingredients": [
                            {
                                "value": 348,
                                "name": "calorie",
                                "desc": "卡路里",
                                "unit": "千卡"
                            },
                            {
                                "value": 7.8,
                                "name": "protein",
                                "desc": "蛋白质",
                                "unit": "克"
                            },
                            {
                                "value": 0.9,
                                "name": "fat",
                                "desc": "脂肪",
                                "unit": "克"
                            },
                            {
                                "value": 77.7,
                                "name": "carbohydrate",
                                "desc": "碳水化合物",
                                "unit": "克"
                            },
                            {
                                "value": 0.9,
                                "name": "dietaryFiber",
                                "desc": "纤维素",
                                "unit": "克"
                            },
                            {
                                "value": 0.06,
                                "name": "vitaminB1",
                                "desc": "维生素B1",
                                "unit": "毫克"
                            },
                            {
                                "value": 7.5,
                                "name": "na",
                                "desc": "钠",
                                "unit": "毫克"
                            }
                        ],
                        "weight": 300,
                        "id": "5b8fbb67f99ffbe3ae5e22f9"
                    }
                ]
            ]
        }
    },
    "message": "成功",
    "status": "ok"
}

```

####请求值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|weight|double|体重(必填)|
|sexName|string|性别(必填)|
|age|int|年龄(必填)|
|height|double|身高(必填)|
|id|int|用户ID(必填)|

* 所有可选参数都可以传空值

####返回值说明
#####data

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|time|结构2|一天当中三餐的集合|

#####结构2

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|breakfast|结构3|早餐|
|lunch|结构3|午餐|
|dinner|结构3|晚餐|


#####结构3
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|id|string|菜品id|
|name|string|菜品名称|
|image|string|菜品图片|
|weight|double|菜品重量|
|ingredients|结构5|营养元素集合|


#####结构5
| 字段名称   | 类型 | 说明 ： <mark>以下营养元素都为每100克的</mark> |
| ------- | --- | :---:  |
|value	|double| 元素值|
|name	|string| 元素名称|
|desc|	string|	元素名称(中文)|
|unit|	string|	单位|






本文档由 [@酷镜](http://www.cools.ai) 提供 




 