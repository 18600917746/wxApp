# 页面跳转
    1. 使用  <navigator src=""></navigator>
        使用 open-type="obj" 
        navigate : 对应 wx.navigateTo 的功能
        redirect	对应 wx.redirectTo 的功能
        switchTab	对应 wx.switchTab 的功能
        reLaunch	对应 wx.reLaunch 的功能
        navigateBack	对应 wx.navigateBack 的功能
    2. 使用   wx.navigateTo({url:""})
# input 值的获取
    1.使用 bindinput='input(event)' event.detail.value 实时获取数据绑定到 data 的变量中
    2.使用 this.setData 设置数据
# 数据设置同步到视图中
    1.使用 setData({}) 同步数据到视图中
# 冒泡与阻止冒泡
    1.跟进绑定事件的方式不用区分
        bind : 冒泡
        catch : 非冒泡
# 公用的设置
    1.数据 : 一般设置到 app.js globalData中 使用 app= getApp() 进行获取 设置
    2.函数 : 一般设置到 app.js
# 公用的代码片段
    1. <view></view> 使用 <includ src=""/>   样式不能同步到
    2. <template name=""></template> 使用 <import src=""/>  只能导入 模板文件 使用 is 进行 模板区分
# 页面之间的传值
    1.使用 get 的 传参方式
        http:www.baidu.com?a=3&b=4
    2.在页面生命周期函数中 onload(option) option 就是 传递的参数
    
# 布局尽量使用 flex 布局
# 