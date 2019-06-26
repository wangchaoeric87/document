# 酷镜接口文档
![Mou icon](http://www.cools.ai/oramirror_cloud/img/blackLogo.png)
[DOC]
>此文档为酷镜营养师提供的根据用户体征、禁忌、疾病等体征信息计算的一日三餐菜谱推荐的解决方案

### 版本号
* **v1.7.1**

### 文档目录
#### 1. 菜谱推荐接口
#### 2. 文本分析菜品接口



### *1、菜谱推荐接口*
#### 功能说明：
根据用户家庭各成员的体征信息返回三餐的食谱
#### 接口地址：


#### 请求参数：
```
[{
	"waist": 40.0,
	"disease": null,
	"weight": 50.0,
	"taboos": "肉",
	"sexName": "女",
	"age": 20,
	"height": 165.0
	"id":121
	"petName":"大眼美女"
}]
```
#### 类型
JSON
#### 请求方式：
POST
#### 返回值：
```
{
    "data": [
        {
            "dish": {
                "lunch": [
                    {
                        "rec_calorie": 0,
                        "pro_protein": 0,
                        "dish": [
                            {
                                "cook_id": 1357304,
                                "rec_reasons": [
                                    "这道菜超多的烟酸让你吃了心情更美丽，还能平衡胆固醇,铁是宝贝健康成长所不能少的必备元素"
                                ],
                                "name": "香喷喷的【番茄土豆烧牛腩】",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 111.82,
                                    "protein": 7.53,
                                    "fat": 4.54,
                                    "carbohydrate": 11.84,
                                    "dietaryFiber": 1.69,
                                    "vitaminA": 32.47,
                                    "vitaminB1": 0.04,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 11.44,
                                    "vitaminE": 0.35,
                                    "niacin": 2.7,
                                    "na": 188.94,
                                    "ca": 11.03,
                                    "fe": 3.38,
                                    "cholesterol": 24.71
                                },
                                "label": [
                                    "富含烟酸",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1554465,
                                "rec_reasons": [
                                    "本道菜富含维生素C是让你成为美女的必备元素"
                                ],
                                "name": "香烤小土豆",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 60.91,
                                    "protein": 2.03,
                                    "fat": 0.23,
                                    "carbohydrate": 12.66,
                                    "dietaryFiber": 1.34,
                                    "vitaminA": 5.4,
                                    "vitaminB1": 0.06,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 20.38,
                                    "vitaminE": 0.26,
                                    "niacin": 1.31,
                                    "na": 156.61,
                                    "ca": 7.4,
                                    "fe": 0.68,
                                    "cholesterol": 0
                                },
                                "label": [
                                    "富含维生素C",
                                    "0胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1608283,
                                "rec_reasons": [
                                    "这道菜超多的铁可以补血养颜，让你脸色红润有光泽,蛋白质多多，营养充足好滋味"
                                ],
                                "name": "风味蹄筋",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 138.62,
                                    "protein": 23.25,
                                    "fat": 1.06,
                                    "carbohydrate": 6.94,
                                    "dietaryFiber": 3.26,
                                    "vitaminA": 75.52,
                                    "vitaminB1": 0.03,
                                    "vitaminB2": 0.11,
                                    "vitaminC": 3.14,
                                    "vitaminE": 1.31,
                                    "niacin": 2.14,
                                    "na": 435.37,
                                    "ca": 43.73,
                                    "fe": 11.51,
                                    "cholesterol": 48.07
                                },
                                "label": [
                                    "富含蛋白质",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1613298,
                                "rec_reasons": [
                                    "本道菜富含维生素E让女人吃了更性感,但是高盐建议大眼美女不宜多吃"
                                ],
                                "name": "美味私房茄子",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 77.88,
                                    "protein": 1.93,
                                    "fat": 2.93,
                                    "carbohydrate": 11.12,
                                    "dietaryFiber": 1.28,
                                    "vitaminA": 12.99,
                                    "vitaminB1": 0.02,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 5.54,
                                    "vitaminE": 2.76,
                                    "niacin": 0.96,
                                    "na": 550.72,
                                    "ca": 38.77,
                                    "fe": 1.91,
                                    "cholesterol": 0
                                },
                                "label": [
                                    "富含维生素E",
                                    "高盐",
                                    "0胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1601073,
                                "rec_reasons": [
                                    "本道菜超多的铁可以补血养颜，让你脸色红润有光泽"
                                ],
                                "name": "素炒三鲜",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 63.26,
                                    "protein": 2.91,
                                    "fat": 0.39,
                                    "carbohydrate": 11.99,
                                    "dietaryFiber": 2.73,
                                    "vitaminA": 106.88,
                                    "vitaminB1": 0.07,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 10.43,
                                    "vitaminE": 0.92,
                                    "niacin": 0.64,
                                    "na": 259.27,
                                    "ca": 47.16,
                                    "fe": 6.22,
                                    "cholesterol": 0
                                },
                                "label": [
                                    "富含铁",
                                    "0胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1345337,
                                "rec_reasons": [
                                    "本道菜超多的维生素A可以抗皱祛斑，让你的肌肤更柔润,但是高脂肪建议大眼美女不宜多吃"
                                ],
                                "name": "红烧肉",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 262.7,
                                    "protein": 5.67,
                                    "fat": 24.63,
                                    "carbohydrate": 4.67,
                                    "dietaryFiber": 0.5,
                                    "vitaminA": 218.35,
                                    "vitaminB1": 0.11,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 3.61,
                                    "vitaminE": 0.47,
                                    "niacin": 1.56,
                                    "na": 45.7,
                                    "ca": 17.28,
                                    "fe": 0.92,
                                    "cholesterol": 68.06
                                },
                                "label": [
                                    "高热量",
                                    "高脂肪",
                                    "富含维生素A",
                                    "低盐"
                                ],
                                "food_type": null
                            }
                        ],
                        "pro_carbohydrate": 0,
                        "pro_fat": 0,
                        "tips": ""
                    }
                ],
                "breakfast": [
                    {
                        "rec_calorie": 0,
                        "pro_protein": 0,
                        "dish": [
                            {
                                "cook_id": 81508,
                                "rec_reasons": [
                                    "本道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,铁是宝贝健康成长所不能少的必备元素,而蛋白质增强肌体免疫力"
                                ],
                                "name": "五彩炒米粉",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 212.58,
                                    "protein": 9.35,
                                    "fat": 3.71,
                                    "carbohydrate": 36.29,
                                    "dietaryFiber": 1.07,
                                    "vitaminA": 140.51,
                                    "vitaminB1": 0.12,
                                    "vitaminB2": 0.08,
                                    "vitaminC": 2.07,
                                    "vitaminE": 0.45,
                                    "niacin": 3.4,
                                    "na": 45.82,
                                    "ca": 15.05,
                                    "fe": 3.55,
                                    "cholesterol": 121.09
                                },
                                "label": [
                                    "高热量",
                                    "富含蛋白质",
                                    "富含烟酸",
                                    "低盐",
                                    "富含铁",
                                    "高胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1575413,
                                "rec_reasons": [
                                    "本道菜超多的烟酸让你吃了心情更美丽，还能平衡胆固醇,铁是宝贝健康成长所不能少的必备元素"
                                ],
                                "name": "宝宝不爱吃蔬菜？或许是还没吃过这道杂蔬小方！",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 120.23,
                                    "protein": 8.98,
                                    "fat": 6.02,
                                    "carbohydrate": 7.82,
                                    "dietaryFiber": 0.45,
                                    "vitaminA": 82.45,
                                    "vitaminB1": 0.05,
                                    "vitaminB2": 0.07,
                                    "vitaminC": 9.3,
                                    "vitaminE": 0.47,
                                    "niacin": 3.67,
                                    "na": 37.51,
                                    "ca": 12.3,
                                    "fe": 3.97,
                                    "cholesterol": 37.06
                                },
                                "label": [
                                    "富含烟酸",
                                    "低盐",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 81508,
                                "rec_reasons": [
                                    "本道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,铁可以补血养颜，让你脸色红润有光泽,而蛋白质吃了能变得更聪明"
                                ],
                                "name": "五彩炒米粉",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 212.58,
                                    "protein": 9.35,
                                    "fat": 3.71,
                                    "carbohydrate": 36.29,
                                    "dietaryFiber": 1.07,
                                    "vitaminA": 140.51,
                                    "vitaminB1": 0.12,
                                    "vitaminB2": 0.08,
                                    "vitaminC": 2.07,
                                    "vitaminE": 0.45,
                                    "niacin": 3.4,
                                    "na": 45.82,
                                    "ca": 15.05,
                                    "fe": 3.55,
                                    "cholesterol": 121.09
                                },
                                "label": [
                                    "高热量",
                                    "富含蛋白质",
                                    "富含烟酸",
                                    "低盐",
                                    "富含铁",
                                    "高胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1623990,
                                "rec_reasons": [
                                    "这道菜富含维生素C是让你成为美女的必备元素,维生素E让女人吃了更性感,但是高盐建议大眼美女不宜多吃"
                                ],
                                "name": "炝薯条",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 152.62,
                                    "protein": 2.74,
                                    "fat": 5.89,
                                    "carbohydrate": 22.35,
                                    "dietaryFiber": 0.82,
                                    "vitaminA": 42.67,
                                    "vitaminB1": 0.05,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 23.69,
                                    "vitaminE": 3.85,
                                    "niacin": 1.22,
                                    "na": 656.57,
                                    "ca": 27.79,
                                    "fe": 2.02,
                                    "cholesterol": 0
                                },
                                "label": [
                                    "富含维生素C",
                                    "富含维生素E",
                                    "高盐",
                                    "0胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1619622,
                                "rec_reasons": [
                                    "本道菜超多的铁可以补血养颜，让你脸色红润有光泽,钙可以强健骨骼，让你身体更健康,而维生素B2是天然护肤养颜的好宝贝,维生素E让男人吃了更强壮,烟酸让你吃了心情更美丽，还能平衡胆固醇"
                                ],
                                "name": "养生番茄鱼片汤",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 64.51,
                                    "protein": 7.79,
                                    "fat": 2.9,
                                    "carbohydrate": 2.59,
                                    "dietaryFiber": 0.31,
                                    "vitaminA": 87.67,
                                    "vitaminB1": 0.17,
                                    "vitaminB2": 0.43,
                                    "vitaminC": 9.8,
                                    "vitaminE": 9.33,
                                    "niacin": 10.86,
                                    "na": 140.15,
                                    "ca": 150.05,
                                    "fe": 3.32,
                                    "cholesterol": 7.18
                                },
                                "label": [
                                    "富含维生素B2",
                                    "富含维生素E",
                                    "富含烟酸",
                                    "富含钙",
                                    "富含铁",
                                    "低胆固醇"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1619600,
                                "rec_reasons": [
                                    "本道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,蛋白质吃了能变得更聪明,而维生素A可以抗皱祛斑，让你的肌肤更柔润"
                                ],
                                "name": "补铁补锌的美味辅食，做一次解决一周配餐！",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 110.45,
                                    "protein": 11.87,
                                    "fat": 4.71,
                                    "carbohydrate": 5.07,
                                    "dietaryFiber": 0.41,
                                    "vitaminA": 256.82,
                                    "vitaminB1": 0.07,
                                    "vitaminB2": 0.15,
                                    "vitaminC": 3.24,
                                    "vitaminE": 1,
                                    "niacin": 4.62,
                                    "na": 59.12,
                                    "ca": 24.62,
                                    "fe": 1.31,
                                    "cholesterol": 202.25
                                },
                                "label": [
                                    "富含蛋白质",
                                    "富含维生素A",
                                    "富含烟酸",
                                    "低盐",
                                    "高胆固醇"
                                ],
                                "food_type": null
                            }
                        ],
                        "pro_carbohydrate": 0,
                        "pro_fat": 0,
                        "tips": ""
                    }
                ],
                "dinner": [
                    {
                        "rec_calorie": 0,
                        "pro_protein": 0,
                        "dish": [
                            {
                                "cook_id": 1616799,
                                "rec_reasons": [
                                    "本道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,铁是宝贝健康成长所不能少的必备元素,而蛋白质吃了能变得更聪明"
                                ],
                                "name": "西红柿蔬菜丸子汤",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 116.17,
                                    "protein": 9.01,
                                    "fat": 7.71,
                                    "carbohydrate": 3.04,
                                    "dietaryFiber": 0.44,
                                    "vitaminA": 97.02,
                                    "vitaminB1": 0.03,
                                    "vitaminB2": 0.09,
                                    "vitaminC": 10.88,
                                    "vitaminE": 0.62,
                                    "niacin": 3.73,
                                    "na": 496.12,
                                    "ca": 32.91,
                                    "fe": 4.29,
                                    "cholesterol": 38.67
                                },
                                "label": [
                                    "富含蛋白质",
                                    "富含烟酸",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1545993,
                                "rec_reasons": [
                                    "本道菜超多的维生素A会让你拥有犀利的眼神！"
                                ],
                                "name": "电压力锅版胡萝卜烧鸡",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 93.43,
                                    "protein": 7.69,
                                    "fat": 4.63,
                                    "carbohydrate": 5.07,
                                    "dietaryFiber": 0.65,
                                    "vitaminA": 418.43,
                                    "vitaminB1": 0.04,
                                    "vitaminB2": 0.05,
                                    "vitaminC": 7.7,
                                    "vitaminE": 1.5,
                                    "niacin": 2.41,
                                    "na": 161.58,
                                    "ca": 23.1,
                                    "fe": 1.19,
                                    "cholesterol": 38.6
                                },
                                "label": [
                                    "富含维生素A"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1643663,
                                "rec_reasons": [
                                    "这道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,铁是宝贝健康成长所不能少的必备元素,而蛋白质吃了能变得更聪明"
                                ],
                                "name": "牛肉土豆咖喱饭＃安记咖喱快手菜＃",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 140.45,
                                    "protein": 11.08,
                                    "fat": 7.7,
                                    "carbohydrate": 7.81,
                                    "dietaryFiber": 0.82,
                                    "vitaminA": 7.19,
                                    "vitaminB1": 0.05,
                                    "vitaminB2": 0.08,
                                    "vitaminC": 11.43,
                                    "vitaminE": 0.27,
                                    "niacin": 4.57,
                                    "na": 120.23,
                                    "ca": 8.17,
                                    "fe": 4.79,
                                    "cholesterol": 46.63
                                },
                                "label": [
                                    "富含蛋白质",
                                    "富含烟酸",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1612124,
                                "rec_reasons": [
                                    "这道菜富含烟酸让你吃了心情更美丽，还能平衡胆固醇,蛋白质吃了能变得更聪明"
                                ],
                                "name": "土豆番茄烧牛腩",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 79.21,
                                    "protein": 11.15,
                                    "fat": 1.64,
                                    "carbohydrate": 4.38,
                                    "dietaryFiber": 0.38,
                                    "vitaminA": 38.68,
                                    "vitaminB1": 0.05,
                                    "vitaminB2": 0.08,
                                    "vitaminC": 9.32,
                                    "vitaminE": 0.79,
                                    "niacin": 3.5,
                                    "na": 344.39,
                                    "ca": 13.52,
                                    "fe": 1.73,
                                    "cholesterol": 28.95
                                },
                                "label": [
                                    "富含蛋白质",
                                    "富含烟酸"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1293705,
                                "rec_reasons": [
                                    "这道菜富含铁是宝贝健康成长所不能少的必备元素,维生素A可以抗皱祛斑，让你的肌肤更柔润"
                                ],
                                "name": "蒜香煎牛扒",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 61.19,
                                    "protein": 5.03,
                                    "fat": 3.14,
                                    "carbohydrate": 3.37,
                                    "dietaryFiber": 0.78,
                                    "vitaminA": 235.42,
                                    "vitaminB1": 0.03,
                                    "vitaminB2": 0.07,
                                    "vitaminC": 16.9,
                                    "vitaminE": 0.5,
                                    "niacin": 2.12,
                                    "na": 56.28,
                                    "ca": 49.12,
                                    "fe": 2.86,
                                    "cholesterol": 18.39
                                },
                                "label": [
                                    "富含维生素A",
                                    "低盐",
                                    "富含铁"
                                ],
                                "food_type": null
                            },
                            {
                                "cook_id": 1651307,
                                "rec_reasons": [
                                    "本道菜超多的维生素A可以抗皱祛斑，让你的肌肤更柔润"
                                ],
                                "name": "咖喱鸡",
                                "weight": 0,
                                "ingredients": {
                                    "calorie": 99.57,
                                    "protein": 5.77,
                                    "fat": 4.94,
                                    "carbohydrate": 7.85,
                                    "dietaryFiber": 0.66,
                                    "vitaminA": 232.29,
                                    "vitaminB1": 0.03,
                                    "vitaminB2": 0.07,
                                    "vitaminC": 13.02,
                                    "vitaminE": 0.96,
                                    "niacin": 2.27,
                                    "na": 282.94,
                                    "ca": 19.22,
                                    "fe": 1.13,
                                    "cholesterol": 50.23
                                },
                                "label": [
                                    "富含维生素A"
                                ],
                                "food_type": null
                            }
                        ],
                        "pro_carbohydrate": 0,
                        "pro_fat": 0,
                        "tips": ""
                    }
                ]
            },
            "day": 1
        },               
         .....
```

#### 请求值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
| waist |double|腰围(可选)|
|disease|string|疾病 用逗号分隔 暂定(可选)|
|weight|double|体重(必填)|
|taboos|string|禁忌标签，用逗号分隔(可选)|
|sexName|string|性别(必填)|
|age|int|年龄(必填)|
|height|double|身高(必填)|
|petName|string|昵称(必填)|
|id|int|家庭ID(必填)|

* 所有可选参数都可以传空值

#### 返回值说明
##### data

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|dish|结构2|一天当中三餐的集合|
|day|int|天数（第几天）|

##### 结构2

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|breakfast|结构3|早餐|
|lunch|结构3|午餐|
|dinner|结构3|晚餐|

##### 结构3

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|rec_calorie|double|建议的卡路里摄入量(当前一餐) <mark>暂时返回0</mark>|
|pro_protein| double |蛋白质功能比 <mark>暂时返回0</mark>|
|dish| 结构4 |当前用户的推荐菜品集合|
|pro_carbohydrate| double |碳水化合物功能比 <mark>暂时返回0</mark>|
|pro_fat| double |脂肪功能比 <mark>暂时返回0</mark>|
|tips|string|说明 (暂时用来提示8岁以下的人群不参与计算)|

##### 结构4
| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
|cook_id|int|菜品id|
|name|string|菜品名称|
|label|list|菜品推荐标签|
|weight|double|菜品重量|
|ingredients|结构5|营养元素集合|
|rec_reasons|string|推荐理由|
|food_type|string|菜品类型|

##### 结构5
| 字段名称   | 类型 | 说明 ： <mark>以下营养元素都为每100克的</mark> |
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


### *2、文本分析菜品接口*
#### 功能说明：
根据一段文本文字返回文本中的`食物`与对应`重量`
#### 接口地址：
* `UClould`：http://123.59.140.18/oramirror_cloud/api/analysisData.do?app_key=app的key
* `阿里云`: http://60.205.107.6/oramirror_cloud/api/analysisData.do?app_key=APP的key

#### 请求参数：
{“name”:“我吃了100克鱼香肉丝”}
#### 类型
JSON
#### 请求方式：
POST
#### 返回值：
```
{“data”:
 {
    "mark": “”,
    “date”：“2017-06-06”，
    “meal”:1,
    "list": [
        [
            {
                    "name": "鱼香肉丝",
                    "id": 1462521086300,
                    "weight": 100,
                    "pic_url": "http://www.oramiro.com/oramirror_cloud/group/114997/1464317238866.jpg"
              }
         ]
    ]
 },
  “msg”:””,
  “code”:”success”
}
```
#### 返回值说明

| 字段名称   | 类型 | 说明  |
| ------- | --- | :---:  |
| mark  | string | 说明|
| weight | double | 重量|
| name | string | 食物名称|
|id | double | 食物id|
|pic_url|string| 食物图片|
|date|string|日期| 
|meal|int|0：没有识别，1：早餐，2：午餐 ，3：晚餐|


本文档由 [@酷镜](http://www.cools.ai) 提供 




