![Logo](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/logo/%E6%A2%A6-128.png?raw=true)


## 周公解梦境 for 微信小程序
![By Leo](https://img.shields.io/badge/Powered_by-Leo-red.svg?style=flat) 
![Libscore](https://img.shields.io/libscore/s/jQuery.svg?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/leochan2017/zgjm.svg)
![Packagist](https://img.shields.io/packagist/l/doctrine/orm.svg)


## 项目地址
[https://github.com/leochan2017/zgjm](https://github.com/leochan2017/zgjm)


## 运行平台
微信小程序

## 扫码体验
来，快点掏出你的大手机，打开微信扫一扫吧

![QR CODE](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/logo/gh_54e23eb8715a_258.jpg?raw=true)



## 界面截图
#### 首页
![截图1](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/%E6%88%AA%E5%9B%BE/1.png?raw=true)

#### 结果页
![截图2](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/%E6%88%AA%E5%9B%BE/2.png?raw=true)

#### 类别页1
![截图3](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/%E6%88%AA%E5%9B%BE/3.png?raw=true)

#### 类别页2
![截图4](https://github.com/leochan2017/zgjm/blob/master/%E7%B4%A0%E6%9D%90/%E6%88%AA%E5%9B%BE/4.png?raw=true)


## 反馈
[提交Issues](https://github.com/leochan2017/ekp-helper/issues/new)


## License
[MIT](http://opensource.org/licenses/MIT)




## 提取组集合

```
var arr = [];

for (i of dreamsData) {
	arr.push(i.group)
}

[...new Set(arr)];

```

## 提取标题集合

```

var groupArr = [];

for (i of dreamsData) {
    groupArr.push(i.group);
}

groupArr = [...new Set(groupArr)];

var bigTiteList = [];

for (itemGroup of groupArr) {
    var itemTitleList = [];
    for (j of dreamsData) {
        if (j.group == itemGroup) {
            itemTitleList.push(j.title);
        }
    }

    itemTitleList = [...new Set(itemTitleList)];

    bigTiteList.push(itemTitleList);
}

bigTiteList = [...new Set(bigTiteList)];

JSON.stringify(bigTiteList);

```