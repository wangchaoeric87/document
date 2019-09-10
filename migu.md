# 酷镜接口文档


>此文档为酷镜营养师提供咪咕语音识别、录入、推荐模块的接口调用及返回值等。

### 版本号
* **v1.0.2**

### 文档目录
#### 1. 语音菜谱推荐接口
#### 2. 语音分析菜品接口



### *1、语音菜谱推荐接口*
#### 功能说明：
语音模块-推荐

根据语音的分析用户记录（推荐），返回的数据根据用户语义解析后推荐一天(一周、一餐)的餐食结果
#### 接口地址：
* `URL`: http://118.190.55.133:9095/getNutritionByName?value=我本周吃点什么

#### 请求参数：
```
{
	"weight": 50.0,
	"sexName": "女",
	"age": 20,
	"height": 165.0,
	"id":121
}
```
#### 类型
JSON
#### 请求方式：
POST
#### 返回值：
```
{
    "data": 
    
        [
        {
            "day": 5,
            "meal": [
                {
                    "type": "breakfast",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fae3d9057c3937719c.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=OYc9d9i6NVjIt5cI54w%2BMkLnWMw%3D",
                                "name": "菜粥",
                                "weight": 200,
                                "ingredients": [
                                    {
                                        "value": 120,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 2.88,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.38,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 24.68,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.66,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 113.79,
                                        "name": "vitaminA",
                                        "desc": "维生素A",
                                        "unit": "微克"
                                    },
                                    {
                                        "value": 343.56,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2fe5fae3d9057c3937719c"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fde3d9057c39377441.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=wv3rU7407vz7vSX1XxEsJ581WYI%3D",
                                "name": "桂花红糖小元宵",
                                "weight": 150,
                                "ingredients": [
                                    {
                                        "value": 510,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 4.35,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 12.94,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 96.42,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.88,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 27.46,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 110.53,
                                        "name": "ca",
                                        "desc": "钙",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2fe5fde3d9057c39377441"
                            }
                        ]
                    ]
                },
                {
                    "type": "lunch",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d740b4cae020770863966.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=lOQFsVMTW3PHDu3gOCVf7thJtaI%3D",
                                "name": "韭菜花炒猪肉",
                                "weight": 70,
                                "ingredients": [
                                    {
                                        "value": 150,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 5,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 12.53,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 4.42,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.27,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.05,
                                        "name": "vitaminB2",
                                        "desc": "维生素B2",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 1243.49,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d740b4cae020770863966"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73a94cae020770862ba0.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=7qRb9rGDlywK2eFfK007g%2FK531o%3D",
                                "name": "黑木耳炒地瓜叶",
                                "weight": 90,
                                "ingredients": [
                                    {
                                        "value": 160,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 1.15,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 15.17,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 6.41,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.12,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 5904.2,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 29.57,
                                        "name": "ca",
                                        "desc": "钙",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73a94cae020770862ba0"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fae3d9057c39377187.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=83oo0ytby06GjDuLEurkePpxCm4%3D",
                                "name": "低糖小贝果",
                                "weight": 150,
                                "ingredients": [
                                    {
                                        "value": 260,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 8.45,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 2.01,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 51.4,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.31,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.37,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 598.19,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2fe5fae3d9057c39377187"
                            }
                        ]
                    ]
                },
                {
                    "type": "dinner",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73274cae0207708618d1.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=dmEmkasDY5cYHjwdElNirpTL5oY%3D",
                                "name": "淡奶油蛋糕",
                                "weight": 60,
                                "ingredients": [
                                    {
                                        "value": 150,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 4.45,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 9.17,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 12.36,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.27,
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
                                        "value": 33.74,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73274cae0207708618d1"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73564cae020770861f8f.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=qny%2FNwoX7Sdms2YaW40qS9%2BEHok%3D",
                                "name": "湖南农家小炒肉",
                                "weight": 50,
                                "ingredients": [
                                    {
                                        "value": 170,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 5.63,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 15.49,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 2.19,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.18,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.45,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 380.86,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73564cae020770861f8f"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73724cae0207708623ca.jpg?Expires=1563963595&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=aj8MqIB47RXCZccXpVeK0cIusOo%3D",
                                "name": "紫薯西米糕",
                                "weight": 150,
                                "ingredients": [
                                    {
                                        "value": 270,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 5.48,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.23,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 59.36,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.41,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.2,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 19.13,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73724cae0207708623ca"
                            }
                        ]
                    ]
                }
            ],
            "type": "normal"
        },
        {
            "day": 6,
            "meal": [
                {
                    "type": "breakfast",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fde3d9057c39377455.jpg?Expires=1563960813&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=jEnI%2FFHVSrtS4zXKzECB6CgXMsM%3D",
                                "name": "小白菜包子",
                                "weight": 150,
                                "ingredients": [
                                    {
                                        "value": 180,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 10.55,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.41,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 33.54,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 3.35,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 7.97,
                                        "name": "vitaminC",
                                        "desc": "维生素C",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 1261.9,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2fe5fde3d9057c39377455"
                            }
                        ]
                    ]
                },
                {
                    "type": "lunch",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73944cae020770862802.jpg?Expires=1563960813&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=X8pBMWmrJ63eZcDgj5c7DiGw%2B5c%3D",
                                "name": "胡萝卜烧口蘑",
                                "weight": 70,
                                "ingredients": [
                                    {
                                        "value": 100,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 11.25,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 14.64,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 5.98,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 12.43,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 465.86,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73944cae020770862802"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d74214cae020770863d70.jpg?Expires=1563960813&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=2oUo6OKSMQbYiFehyoGHTJMZgfc%3D",
                                "name": "南瓜烧土豆",
                                "weight": 270,
                                "ingredients": [
                                    {
                                        "value": 90,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 3.17,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.38,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 21.4,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 2.53,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1816.67,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 1.25,
                                        "name": "fe",
                                        "desc": "铁",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d74214cae020770863d70"
                            }
                        ]
                    ]
                },
                {
                    "type": "dinner",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d74254cae020770863e49.jpg?Expires=1563960813&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=TUMxGQ6BGyfRI%2B55rPJObUHXxDk%3D",
                                "name": "西红柿炒辣椒",
                                "weight": 420,
                                "ingredients": [
                                    {
                                        "value": 100,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 3.83,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.77,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 22.88,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 5.45,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.27,
                                        "name": "vitaminE",
                                        "desc": "维生素E",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 25.29,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d74254cae020770863e49"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d741a4cae020770863c3a.jpg?Expires=1563960813&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=KlhlFB8HETiOx6OvfiEi%2FiCcRrg%3D",
                                "name": "西红柿蒸猪肝",
                                "weight": 160,
                                "ingredients": [
                                    {
                                        "value": 100,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 8.11,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 4.2,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 9.85,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 2.51,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 4.21,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 463.49,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d741a4cae020770863c3a"
                            }
                        ]
                    ]
                }
            ],
            "type": "light"
        },
        {
            "day": 7,
            "meal": [
                {
                    "type": "breakfast",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2fe5fde3d9057c3937742d.jpg?Expires=1563960807&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=ry0moxt9SasXsu7hsAd43p9opX4%3D",
                                "name": "蒜香瓜条",
                                "weight": 150,
                                "ingredients": [
                                    {
                                        "value": 150,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 3.96,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 11.69,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 9.69,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 4.24,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 15.86,
                                        "name": "vitaminA",
                                        "desc": "维生素A",
                                        "unit": "微克"
                                    },
                                    {
                                        "value": 2232.61,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2fe5fde3d9057c3937742d"
                            }
                        ]
                    ]
                },
                {
                    "type": "lunch",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d74314cae0207708640a9.jpg?Expires=1563960807&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=SpTzYwf7eN7P888JRidmwJlM3bA%3D",
                                "name": "茭白炒鱿鱼",
                                "weight": 450,
                                "ingredients": [
                                    {
                                        "value": 90,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 5.35,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.72,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 20.01,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 6.25,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 118.13,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 17.86,
                                        "name": "ca",
                                        "desc": "钙",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d74314cae0207708640a9"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d742b4cae020770863f6e.jpg?Expires=1563960807&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=fLeSIQSbKDMkPUCo%2FOM2oQDaRoU%3D",
                                "name": "胡萝卜炒木耳",
                                "weight": 110,
                                "ingredients": [
                                    {
                                        "value": 110,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 1.38,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 9.35,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 6.78,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 2.32,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.29,
                                        "name": "niacin",
                                        "desc": "烟酸",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 4197.41,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d742b4cae020770863f6e"
                            }
                        ]
                    ]
                },
                {
                    "type": "dinner",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d74244cae020770863e11.jpg?Expires=1563960807&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=s%2FIGjmcslksQpj0OnZUMI1TynBY%3D",
                                "name": "金针菇炒西红柿",
                                "weight": 210,
                                "ingredients": [
                                    {
                                        "value": 100,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 10.93,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.65,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 14.3,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 4.47,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 3951.16,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 22.28,
                                        "name": "ca",
                                        "desc": "钙",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d74244cae020770863e11"
                            },
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d73ad4cae020770862c76.jpg?Expires=1563960807&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=nXdSlvwHFza72IbcZ0i9ZlIa5jc%3D",
                                "name": "韭菜炒土豆丝",
                                "weight": 100,
                                "ingredients": [
                                    {
                                        "value": 100,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 7.23,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.47,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 18.4,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.92,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.02,
                                        "name": "vitaminB2",
                                        "desc": "维生素B2",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 4303.67,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    }
                                ],
                                "id": "5d2d73ad4cae020770862c76"
                            }
                        ]
                    ]
                }
            ],
            "type": "light"
        }
    ],
    "message": "成功",
    "type": 2,
    "status": "ok"
}

```

#### 请求值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|weight|double|体重(必填)|
|sexName|string|性别(必填)|
|age|int|年龄(必填)|
|height|double|身高(必填)|
|id|int|用户ID(必填)|

* 所有可选参数都可以传空值

#### 返回值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|data|data|数据集合|
|message|string|返回成功或失败的信息|
|status|string|状态|
|type|int|2:推荐 1：记录（本次语义分析后得出的语义类型）|



##### data

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|day|String|时间:当类型为推荐时，day会返回序号，当类型为记录时，day返回的是日期|
|meal|结构2|一天当中三餐的集合|
|type|String|类型：(断食light、正常normal)|

##### 结构2

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|type|string|三餐标示，（早、 中、 午餐）|
|data|结构3|食谱集合|



##### 结构3
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|id|string|菜品id|
|name|string|菜品名称|
|image|string|菜品图片|
|weight|double|菜品重量|
|ingredients|结构5|营养元素集合|


##### 结构5
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|value	|double| 元素值|
|name	|string| 元素名称|
|desc|	string|	元素名称(中文)|
|unit|	string|	单位|


### *2、语音分析菜品接口*
#### 功能说明：
语音模块-记录

根据一段文本文字返回文本中的`食物`与对应`重量`，集合中包含相似的5道菜品，识别概率从高到底。开发者只需要从集合中取出第一个元素作为识别后的菜品即可，其余菜品可以做用户手动选择项，
#### 接口地址:

* `URL`: http://118.190.55.133:9095/getNutritionByName?value=我今天早上吃了一碗粥中午吃了200克鱼香肉丝和一碗大米饭

#### 请求参数：
	{
	  "weight": 70.0, 
	  "sexName": "男",
	  "age": 27,
	  "height": 171.0,
	  "id":1
	}
#### 类型
JSON
#### 请求方式：
POST
#### 返回值：
```
{
    "data": [
        {
            "meal": [
                {
                    "type": "breakfast",
                    "data": [
                        [
                            {
                                "image": null,
                                "name": "粥",
                                "ingredients": [
                                    {
                                        "value": 160,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 3.85,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.05,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 34.65,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 0.35,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 9.8,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 0,
                                        "name": "cholesterol",
                                        "desc": "胆固醇",
                                        "unit": "毫克"
                                    }
                                ],
                                "weight": 350,
                                "id": "5b8fbb67f99ffbe3ae5e22fd"
                            }
                        ]
                    ]
                },
                {
                    "type": "lunch",
                    "data": [
                        [
                            {
                                "image": "http://kujingimage.oss-cn-beijing.aliyuncs.com/5d2d730e4cae02077086146e.jpg?Expires=1563963972&OSSAccessKeyId=LTAI9QL9miIJuL3L&Signature=zJchTrj%2BbNIP5iPDGg3CA66%2FVIQ%3D",
                                "name": "鱼香肉丝",
                                "weight": 200,
                                "ingredients": [
                                    {
                                        "value": 550,
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
                                        "value": 1.62,
                                        "name": "vitaminC",
                                        "desc": "维生素C",
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
                            }
                        ],
                        [
                            {
                                "image": "http://app.oramiro.com:8082/oramirror_cloud/group/114997/1464266101204.jpg",
                                "name": "大米饭",
                                "ingredients": [
                                    {
                                        "value": 410,
                                        "name": "calorie",
                                        "desc": "卡路里",
                                        "unit": "千卡"
                                    },
                                    {
                                        "value": 9.1,
                                        "name": "protein",
                                        "desc": "蛋白质",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.05,
                                        "name": "fat",
                                        "desc": "脂肪",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 90.65,
                                        "name": "carbohydrate",
                                        "desc": "碳水化合物",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 1.05,
                                        "name": "dietaryFiber",
                                        "desc": "纤维素",
                                        "unit": "克"
                                    },
                                    {
                                        "value": 8.75,
                                        "name": "na",
                                        "desc": "钠",
                                        "unit": "毫克"
                                    },
                                    {
                                        "value": 4.55,
                                        "name": "fe",
                                        "desc": "铁",
                                        "unit": "毫克"
                                    }
                                ],
                                "weight": 350,
                                "id": "5b8fbb67f99ffbe3ae5e22f9"
                            }
                        ]
                    ]
                }
            ],
            "day": "2019-07-24"
        }
    ],
    "message": "成功",
    "type": 1,
    "status": "ok"
}

```

#### 请求值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|weight|double|体重(必填)|
|sexName|string|性别(必填)|
|age|int|年龄(必填)|
|height|double|身高(必填)|
|id|int|用户ID(必填)|

* 所有可选参数都可以传空值

#### 返回值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|data|data|数据集合|
|message|string|返回成功或失败的信息|
|status|string|状态|
|type|int|2:推荐 1：记录（本次语义分析后得出的语义类型）|



##### data

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|day|String|时间:当类型为推荐时，day会返回序号，当类型为记录时，day返回的是日期|
|meal|结构2|一天当中三餐的集合|
|type|String|类型：(断食light、正常normal)|

##### 结构2

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|type|string|三餐标示，（早、 中、 午餐）|
|data|结构3|食谱集合|



##### 结构3
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|id|string|菜品id|
|name|string|菜品名称|
|image|string|菜品图片|
|weight|double|菜品重量|
|ingredients|结构5|营养元素集合|


##### 结构5
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|value	|double| 元素值|
|name	|string| 元素名称|
|desc|	string|	元素名称(中文)|
|unit|	string|	单位|



### 可返回的营养数据类型一览表

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|calorie	|double|	卡路里|
|protein	|double|	蛋白质|
|carbohydrate|	double|	碳水化合物|
|fat|	double|	脂肪|
|dietaryFiber|	double|	膳食纤维|
|na	|double|	钠|
|ca	|double|	钙|
|fe	|double|	铁|
|niacin|	double|	烟酸|
|cholesterol|	double|	胆固醇|
|vitaminA	|double|	维生素A|
|vitaminB1|	double	|维生素B1|
|vitaminB2|	double	|维生素B2|
|vitaminC	|double	|维生素C|
|vitaminE|	double	|维生素E|


本文档由 [@酷镜](http://www.cools.ai) 提供 




 
