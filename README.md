# Shadowrocket 配置文件

本项目是维护一个Shadowrocket配置文件

其中翻墙部分规则是将[GfwList](https://github.com/gfwlist/gfwlist)转化而得来，屏蔽广告部分规则是根据[easylist_adservers](https://github.com/easylist/easylist/blob/master/easylist/easylist_adservers.txt)和
[easylist_thirdparty](https://github.com/easylist/easylist/blob/master/easylist/easylist_thirdparty.txt)的规则转化而来

>* gfwlist->  ```DOMAIN-SUFFIX,rule,Proxy```
>* easylist-> ```DOMAIN-SUFFIX,rule,REJECT```

## 如何使用项目

``` Python
python main.py 
```
生成的规则存放在 ```rule.txt``` 和 ```rulewithad.txt```两个文件之中。第一个是单纯的翻墙配置文件，第二个在翻墙基础之上加入了屏蔽广告部分规则。

## 使用翻墙的配置文件

打开Shadowrocket，添加配置文件，写入下面的链接
 
url:  https://raw.githubusercontent.com/Hsiny/Shadowrocket-Config/master/rule.txt

或者直接扫描下面的二维码

![QR code](png/proxy.png)

## 使用翻墙和屏蔽广告的配置文件

打开Shadowrocket，添加配置文件，写入下面的链接 
 
url:  https://raw.githubusercontent.com/Hsiny/Shadowrocket-Config/master/rulewithad.txt

或者直接扫描下面的二维码

![QR code](png/proxyandadblock.png)


## To do
>* ~~add ad block rules~~
>* ~~fix some regex rules in gfwlist~~
>* ~~add other easylist ad-block rulus~~
>* ~~add some rules to block ads~~
>* reduce the number of ad-block rules





