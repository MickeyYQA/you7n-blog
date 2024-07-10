---
layout: post
title: 竞赛做网站曲折经历.html
date: 2024-01-13 19:32 +0800
tags: [html, supersmest, conrad]
toc:  true
---

现在是2024年1月13号下午五点，本蒟蒻刚刚搞完ddl在15号的Conrad竞赛的网站。解决了应该是所有问题，还是挺开心的（打滚）。想记一下做这个网站的神奇妙妙经历。
{: .message }

## 9月26日
故事从9月26号开始——
九月底同学问我要不要参加Conrad，让我负责做网站和做视频。我寻思这不简单吗就说好啊搞呗。
最开始想偷懒，就拿了之前给一个Minecraft服务器做主页用下的html模版填吧填吧放上线了。大概长这样，看起来酷酷的。
![placeholder](https://raw.githubusercontent.com/MickeyYQA/you7n-blog/master/img/20240113/wps_doc_0.jpg "img")
当时我组还没有很确定研究主题和内容，所以网站上的内容都是lorem ipsum。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_1.jpg "img")
（这个挺搞笑）
## 10月10日
此时时间进行到了10月10日——
后来在租服务器的地方整了个他们的二级域名 (类似supersmest.[他们服务器的名字].com这样的)，用起来还挺流畅就没怎么管。突然有一天不行了，网站上去会报错。不是'http error'，是弹出窗口提示的（到现在也没搞清楚是为什么）。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_2.jpg "img")
又后来一天，二级域名上不去了。去服务器那一查发现他们不再提供二级域名分发服务了。（刚才上去又看了一眼怎么又有了。。。反正当时肯定是没有）我看这个寄了那我就得自己买个域名了啊，遂去阿里云买域名。
## 11月26日
此时时间进行到了11月26号——

因为组名叫supersmest吗，于是果断买了supersmest.com。这个域名上去会显示无法访问此网站阿、检查 supersmest.com 中是否有拼写错误阿、DNS_PROBE_FINISHED_NXDOMAIN阿什么的。这个过会说。然后把之前那个fancy的模版放了上去，非常成功非常顺利，只是还是会弹窗错误。

然后就在搞网站备案，因为是在阿里云买的网站。搞了半天搞不定太麻烦了就扔一边了。当时想的是 看起来网站不完成备案也还可以访问 应该没什么大问题吧。
随后的一个月都在本地写点网站内容什么的。
## 1月2日
此时时间进行到了1月2号——
（通过时间进行的速度你可以看出最开始的这么久荒废了多少时间，，）此时距离ddl还有13天，大家终于意识到我们时间不太够了。于是这天早上语文课找班主任请了两节课假狠狠的搞conrad。我突然意识到我之前那个弹窗的问题还没有解决，应该是模版的问题，于是迅速找了新的模版。比原来那个还酷而且还不报错。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_3.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_4.jpg "img")
这个模版的动画特别好看。上面这个是随便改了改的成果。
## 1月3日
此时时间进行到了1月3号——

上午组长L同学找我，说希望在网页上加一个可以拖转旋转和放大缩小的3D模型，模型她做，我搞前端。据说是长得像这样的东西
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_5.jpg "img")
当时就说这东西是不是太fancy了，我不会啊。她说你就做吧。
我就到处找可以在网页前端放模型的东西，找到了x3dom这个库。研究了半天搞出来个方块
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_6.jpg "img")
后来才发现这玩意不能导入模型!!总不能我在html里复刻一个那个模型吧。于是去找其他解决办法。
然后3号还把网站填了填：
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_7.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_8.jpg "img")
这个时候已经初见雏形了，这个背景图是现在用的背景图，Intro里面的第一段话现在还在只是换了地方。
## 1月5日
时间进行到了1月5号——

在我的一番研究下找到了three.js这个神奇的东西，可以在网页前端加载gltf模型。浏览器搜了几个就开始自己做。

下面遇到的问题记不清时间了，总之是1月5号到1月7号之间遇到的所有问题。
先搓了一个js，发现根本用不了。找AI也解决不了问题。于是去网上找各种gltf loader网站，试图扒他们源代码下来，也以失败告终。还是老老实实去网上找解决办法和现成的代码，发现这玩意根本没有现成的代码。能用的全都一个样，文件处理都在本地，没有一个link能内嵌到我的网站里的。

继续和AI一起手搓js改问题。发现之前的代码里用到的「GLTFLoader」和「three.js」不是一个版本的，找到了解决办法把这个问题解决了。
之前根本用不了的代码都是一片白，用chrome右键可以检查 看得到报错信息，这个打开html后是黑的。虽然也还是不行，但是本蒟蒻欣喜若狂，认为这是成功一半的征兆。
在网上搜到说这个东西不能在本地运行，于是用python和flask库开了个局域网服务器。后来发现这个东西只能引用index.html一个文件，剩下的模型文件他访问不到，报404。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_9.jpg "img")
然后就试图把这个放在租的服务器上调试。调试的第一天晚上是正常的全黑页面，第二天出现了一点小状况。
## 1月8日
此时时间进行到了1月8号上午——

在学校收到阿里云的一封邮件，一看慌了。距离ddl还有五天了突然给我整这出 把没有备案的事情忘得一干二净。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_10.jpg "img")
于是赶紧跑去阿里云搞备案，非常不顺利。
先是正常流程去备案，阿里云告诉我
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_11.jpg "img")
仔细想了一下，域名实名认证填的是我自己的信息，备案主体信息填的是我妈的（因为它最开始在我填写域名实名认证的时候没告诉我什么未成年人不能填写，后来在填主体信息的时候说未成年人不行要填成年人的 我就填了我妈的）。最开始没想到这玩意还会影响。于是按照它的提示给我账号过户给我妈。（此处鸣谢我妈赞助买两个域名和备案的钱 因为本人支付宝没钱）
过户完提示我
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_12.jpg "img")
这个也太有病了。。。强烈提倡通信管理局提高工作效率。
总之就是没有在当天晚上六点前把备案搞完，阿里云把我supersmest.com的域名解析停了。这就是为什么你现在访问它访问不上去。
我也没有继续完成备案的意愿，因为备案完成至少需要7到13天，最早就是在ddl当天备案完，根本没时间调试新东西。
于是我的解决办法是，卡他域名注册的40天无敌时间。9号立刻买了新的域名（supersmest.top 这个便宜），这样至少能在29号出结果前没有任何问题。
## 1月9日
此时时间进行到了1月9号——

gltf loader的问题很大，我自己搞不定。我爸说他可以问问他公司搞前端的同事。（暂且称之为同事先生吧。）
## 1月10日
此时时间进行到了1月10号——

同事先生有消息了，帮我刷刷刷改成一个能用的gltf loader（大感激orz）。虽然有一点小问题吧，至少加载出来了。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_13.jpg "img")
我自己同时在改html，往上加东西。写了不少。
## 1月11日
此时时间进行到了1月11号上午——

修改了模型，但是不能加载材质。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_14.jpg "img")
不加载材质似乎是gltf loader的通病，搜索引擎能搜到的轻量loader都不加载.bin材质文件。所以不管这个问题，直接用了。（再感谢同事先生）
此时时间进行到了1月12号，也就是昨天——

想起来应该再充实一下网站上的科研部分的内容，于是找负责计算的M同学要了计算过程和数据，用一个LaTeX编辑器转成了html，放到了网站上。同时在网站上内嵌了一个YouTube视频，还增加和修改了其他内容。
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_15.jpg "img")

这LaTeX放本地看起来格式还挺好看的。
## 1月13日
### 上午
此时时间进行到了1月13号早上——

突然发现网站加载变得难以忍受的慢，而且偶尔还会格式错误。加载主站需要20多秒，加载模型需要40多秒。这谁能忍？

于是根据我爹的建议，从2.0版本开始一个版本一个版本的放到服务器上往后推，看是哪天哪个版本哪个功能出现了问题。正好我在服务器上保存了之前所有的文件，于是开始推。
推到一半发现是从2.3版本开始变得特别慢，当前版本是2.5。2.3是12号下午加完LaTeX和YouTube内嵌后的版本。合理推测是LaTeX公式渲染太慢了导致主站打开特别慢。于是把LaTeX公式变成了图片（虽然这样看起来难看一些）

![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_16.jpg "img")

### 下午
时间进行到1月13号下午，也就是现在——

改完LaTeX发现比原来快了一点，但是还是慢。合理推测是内嵌YouTube视频导致加载变慢。于是把YouTube视频改为点击跳转的按钮，网站加载速度一下就提上来了。
稍微修改了一下格式和内容，应该是再没有东西要改了。我感觉就是完美😎。

btw大家现在也可以去网站上看看，真的很酷炫。点击网址 [http://supersmest.top/](http://supersmest.top/) 就可以进去了！
一些主要页面:
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_17.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_18.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_19.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_20.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_21.jpg "img")
![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_22.jpg "img")
我组的M同学（就是负责搞电压计算的那哥们）写了一首诗
<em></br>I met a traveller from a distant shore,</br>
<em>Who said -- “Two chambers filled with salt and water</br>
Lie in the ocean. . . . Near them, on the floor,</br>
A membrane separates the solutions, whose power,</br>
And voltage difference, and flow of electric charge,</br>
Tell that its inventor well those forces harnessed</br>
Which yet sustain, impressed on these ingenious things,</br>
The hand that made them, and the mind that blessed;</br>
And on the device, these words appear:</br>
My name is Concentration Cell, King of Cells;</br>
Look on my Works, ye Mighty, and revere!</br>
Nothing beside remains. Around the sway</br>
Of that colossal Cell, boundless and fair</br>
The waves and currents dance and play.”</em>

哦对 本蒟蒻在做网站的同时还负责剪视频。视频在网站的YouTube链接里，可能需要魔法一下。考虑到大家是霍格沃茨毕业学员的人数占比比较低，下面这里也可以看视频😋
这个「Supersmest启动」的图标也是本蒟蒻做的😎

![placeholder](https://github.com/MickeyYQA/you7n-blog/blob/4e2ff5eaf46e4c4df1f5e8ba1e150741876cd730/img/20240113/wps_doc_23.jpg "img")
