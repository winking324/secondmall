## 看了几天python，想着做一个东西出来，就做出了一个小型*二手* 商城练练手
### 2020/05/05 更改界面样式 更好看
csdn 地址 https://blog.csdn.net/over110522/article/details/83933039 可以看到效果图
### 2020/03/23 更新sql文件

### 管理员商品审核操作后刷新页面 广告时间改为每小时的第22分钟和53分钟 广告更换 404页面转到index页面 2020/03/23
### 重新增强redis的用处 把热门商品 新品也放在redis中 加入定时任务来更新redis中热门商品数据 修复Admin任何人都可以进入的权限 2020/03/22

### 购物车失效时间计算BUG 已提交最新的代码 2020/03/22
### 新增加管理员审核页面 2020/02/26

https://img-blog.csdnimg.cn/20200226122444724.png

https://img-blog.csdnimg.cn/20200226122603190.png
### 1.解释 
**以下的*二手* 商城展示，商品照片为了好看，从京东上爬下来的，有一些动态效果，我只制作了一张，在线转换成gif的话由于录制屏幕视频文件太大不太容易转格式**

### 2.用户在没有登录的时候点击买东西，会弹出首先登录，同时也可以选择注册
https://img-blog.csdnimg.cn/20181110202812635.png
### 3.卖东西的界面使用了可以拖拽的方式让用户上传商品更方便
https://img-blog.csdnimg.cn/20181110202928861.png
### 4.用户添加商品到购物车的界面，由于二手商品数量每件比较少，所以限定用户在提交到购物车20分钟内完成结算，否则商品会从购物车内清除
https://img-blog.csdnimg.cn/20181110203102771.gif
### 5.加入购物车之后，用户可以去个人中心查看(顺便展示一下更换照片的界面)
https://img-blog.csdnimg.cn/20181110203547493.png
### 6. 这个时候商品已经在你的购物车内，你在个人中心也可以看到购物车并且去结算

https://img-blog.csdnimg.cn/20181110203756381.png
### 7. 去结算
https://img-blog.csdnimg.cn/20181110203830590.png
### 8. 如果用户没有完成结算的话，会在订单中，同样也有时间限制，每件商品都有根据当初进入订单那个时间算起至三十分钟后自动从订单中取消
https://img-blog.csdnimg.cn/20181110204036928.png
### 9. 商品列表页面
https://img-blog.csdnimg.cn/20181110204127316.png
### 10. 在二手商城中难免有些买家觉着卖家定价不合适，会跟商家交谈，所以我也做了一个商品议价的模块，可以实现回复再回复的问题
https://img-blog.csdnimg.cn/20181110204419137.png
### 11.我的总结：

 1. 上面只是简单的页面展示，具体代码在github上，这个项目中有很多的知识点
 2. 希望大家又遇到同样的功能不知道怎么实现的时候，我的代码能够帮到你
 3. 调bug是一件培养心态的一件事，做web也有二年左右了，感觉从代码中培养了好性格

### 11.github地址是:https://github.com/lmx110522/nyist_python_secondmall.git
欢迎访问我的[个人博客](https://www.limaozhan.cn)。
上面的页面可能不太好看，我是一个写后端代码的小码农却喜欢做前台页面，我去努力进步的！，希望你的支持，谢谢花费时间看我的博客，万分感谢！
